project(unity_test_toolkits)

make_boost_test (supervised_learning_mock_test_model.cxx
  REQUIRES supervised_learning)
make_boost_test(logistic_regression_tests.cxx
  REQUIRES supervised_learning)
make_boost_test(linear_regression_tests.cxx
  REQUIRES supervised_learning)
make_boost_test(boosted_trees_classifier_tests.cxx
  REQUIRES supervised_learning sframe)
make_boost_test (random_forest_tests.cxx
  REQUIRES supervised_learning sframe)
make_boost_test(linear_regression_bench.cxx
  REQUIRES supervised_learning)
make_boost_test (linear_svm_tests.cxx
  REQUIRES supervised_learning)
make_boost_test (xgboost_tests.cxx
  REQUIRES xgboost parallel logger)
