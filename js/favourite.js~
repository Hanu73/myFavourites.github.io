var app = angular
    .module('favoriteApp', ['ngMaterial', 'ngMdIcons', 'xeditable'])
    .config(function($mdThemingProvider) {
        $mdThemingProvider.theme("default").primaryColor("blue").accentColor("red");
    }).controller('favCtrl', function($scope, $filter) {
        $scope.user = {
            name: 'awesome user'
        };
        $scope.items = [{
            'name': 'john',
            'phone': '1234567890',
            'address': 'texas',
            'id': 1
        }, {
            'name': 'Mike',
            'phone': '49739243999',
            'address': 'texas',
            'id': 2
        }, {
            'name': 'smith',
            'phone': '132434932993',
            'address': 'texas',
            'id': 3
        }, {
            'name': 'williams',
            'phone': '4323243242378',
            'address': 'texas',
            'id': 4
        }, {
            'name': 'chris',
            'phone': '213123213219',
            'address': 'texas',
            'id': 5
        }]
        $scope.favourites = [];

        $scope.addContact = function() {
            $scope.contact = {
                id: $scope.items.length + 1,
                name: '',
                phone: null,
                address: null
            };
            $scope.items.push($scope.contact);
        };


        // remove contact
        $scope.removeContact = function(index) {

            $scope.items.splice(index, 1);
        };
        $scope.addToFavourites = function(item) {
            $scope.selectedId = item.id;
            var object_by_id = $filter('filter')($scope.favourites, {
                'id': item.id
            })[0];

            if (!object_by_id) {
                $scope.favourites.push(item);


            } else {

                for (var i = 0; i < $scope.favourites.length; i++) {
                    if ($scope.favourites[i].id === item.id) {
                        $scope.favourites.splice(i, 1);

                    }
                }

            }

        }


    })

app.run(function(editableOptions) {
    editableOptions.theme = 'bs3'; // bootstrap3 theme. Can be also 'bs2', 'default'
});
