load('//tools/bzl:gwt.bzl', 'gwt_genrule', 'gen_ui_module',
     'gwt_user_agent_permutations')
load('//tools/bzl:license.bzl', 'license_test')

gwt_genrule()
gwt_genrule('_r')

gen_ui_module(name = 'ui_module')
gen_ui_module(name = 'ui_module', suffix = '_r')

gwt_user_agent_permutations()

license_test(
  name = "ui_module_license_test",
  target = ":ui_module",
)
