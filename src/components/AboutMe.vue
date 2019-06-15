<template>
    <div>
        <section>
            <h1>Biography</h1>
            <p>
                本名 鳩間 大也(hatoma daiya). 沖縄出身, 滋賀で活動するwebエンジニア</br>
                ドキュメントなしの状態でコードを読み解く苦行に一定の経験があります.</br>

            </p>
        </section>

        <section>
            <h1>Career</h1>
            <li v-for="(career, key) in careers" :key="key">
                <span>{{career['term']}}~ {{career['title']}}</span>
                <ul>
                    <li v-for="(useLanguage, key) in career['languages']" :key="key">
                        {{useLanguage}}
                    </li>
                </ul>
            </li>  
            <!-- <li>2015/04~ 製造業向け 生産管理システム 導入   </li>
                <ul>
                    <li>CakePHP3</li>
                </ul>
            <li>2017/04~ 生産管理システム用 APIサーバー導入 </li>   
                <ul>
                    <li>Laravel5.1</li>
                </ul>
            <li>
            <li>2019/06~ このポートフォリオを作成</li>
                <ul>
                    <li>Laravel5.8</li>
                    <li>Vue2.5</li>
                </ul>    -->
        </section>
    </div>
</template>

<script>
export default {
    data() {
        return {
            careers : 
            [
                {
                    'title' : '製造業向け 生産管理システム導入',
                    'term'  : '2015/04',
                    'languages' : [
                        'CakePHP3',
                    ]
                },
                {
                    'title' : '生産管理システム用 APIサーバー導入',
                    'term'  : '2017/04',
                    'languages' : [
                        'Laravel5.1',
                    ]
                },
                {
                    'title' : 'このポートフォリオを作成',
                    'term'  : '2019/06',
                    'languages' : [
                        'laravel5.8',
                        'Vue2.5',
                    ]
                }
            ]
        }
    }
}
</script>   