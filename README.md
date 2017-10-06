# gradle-dependencies-pack
library list + some gradle configuration 


apply plugin: 'kotlin-android'
apply plugin: 'kotlin-android-extensions'
apply plugin: 'realm-android'


ext {
    supportLibraryVersion = '26.0.0-alpha1'
    playServicesVersion = '9.2.1'
    retrofitVersion = '2.3.0'
}

dependencies {
    compile fileTree(dir: 'libs', include: ['*.jar'])
    androidTestCompile('com.android.support.test.espresso:espresso-core:2.2.2', {
        exclude group: 'com.android.support', module: 'support-annotations'
    })
    compile 'com.android.support:appcompat-v7:25.3.0'
    testCompile 'junit:junit:4.12'
    compile "org.jetbrains.kotlin:kotlin-stdlib:$kotlin_version"
    compile 'com.squareup.retrofit2:retrofit:2.1.0'
    compile 'com.squareup.retrofit2:converter-gson:2.1.0'
    compile 'com.squareup.okhttp3:logging-interceptor:3.4.2'
    compile 'org.jetbrains.anko:anko-sdk23:0.9.1'
    compile "com.squareup.retrofit2:retrofit:$retrofitVersion"
    compile "com.squareup.retrofit2:converter-gson:$retrofitVersion"
    compile 'com.squareup.okhttp3:okhttp:3.6.0'
    compile 'com.github.bumptech.glide:glide:3.7.0'
    compile 'com.squareup.okhttp3:logging-interceptor:3.6.0'
    compile 'com.google.code.gson:gson:2.7'   
}
