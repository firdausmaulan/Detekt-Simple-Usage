# Detekt-Simple-Usage
simple usage of detekt library for static code analyze

Put this folder on your project & run it :D

# HELP
java -jar detekt/detekt-cli-1.0.0-RC12-all.jar --help

# FILTER
java -jar detekt/detekt-cli-1.0.0-RC12-all.jar --filters ".*detekt.*";".*test.*";".*androidTest.*"

# CUSTOM CONFIG
java -jar detekt/detekt-cli-1.0.0-RC12-all.jar -c /detekt/custom-detekt-config.yml -f ".*detekt.*";".*test.*";".*androidTest.*"

# REPORTS
java -jar detekt/detekt-cli-1.0.0-RC12-all.jar -r html:detekt/reports/[date].html

java -jar detekt/detekt-cli-1.0.0-RC12-all.jar -f ".*detekt.*";".*test.*";".*androidTest.*" -r html:detekt/reports/[date].html

If you want better report management date should be yyyy_mm_dd
Example : 
java -jar detekt/detekt-cli-1.0.0-RC12-all.jar -f ".*detekt.*";".*test.*";".*androidTest.*" -r html:detekt/reports/2019_01_08.html

# REPORTS WITH CUSTOM CONFIG
java -jar detekt/detekt-cli-1.0.0-RC12-all.jar -c /detekt/custom-detekt-config.yml -f ".*detekt.*";".*test.*";".*androidTest.*" -r html:detekt/reports/2019_01_08.html
