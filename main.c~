#include "zend.h"
#include "zend_extensions.h"
#include "zend_modules.h"
#include "zend_constants.h"
#include "zend_list.h"
#include "zend_API.h"
#include "zend_builtin_functions.h"
#include "zend_ini.h"
#include "diablo/test.h"


#ifdef ZTS
#    define GLOBAL_FUNCTION_TABLE    global_function_table
#    define GLOBAL_CLASS_TABLE        global_class_table
#    define GLOBAL_CONSTANTS_TABLE    global_constants_table
#    define GLOBAL_AUTO_GLOBALS_TABLE    global_auto_globals_table
#else
#    define GLOBAL_FUNCTION_TABLE    CG(function_table)
#    define GLOBAL_CLASS_TABLE        CG(class_table)
#    define GLOBAL_AUTO_GLOBALS_TABLE    CG(auto_globals)
#endif

test_opScan();
if (EG(active_op_array)) {
            EG(return_value_ptr_ptr) = retval ? retval : &local_retval;
            destroy_op_array(EG(active_op_array));
            efree(EG(active_op_array));
        } else if (type==ZEND_REQUIRE) {
            va_end(files);
            EG(active_op_array) = orig_op_array;
            return FAILURE;
        }
    }
    va_end(files);
    EG(active_op_array) = orig_op_array;

    return 0;
}
