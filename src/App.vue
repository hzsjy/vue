<template>
  <div id="app">

    <div id="left"> 
      <el-row class="tac">
        <el-col>   
          <el-menu
            default-active="2"
            class="el-menu-vertical-demo"
            @open="handleOpen"
            @close="handleClose"
            background-color="#304156"
            text-color="#fff"
            active-text-color="#ffd04b">

            <el-menu-item index="1">
              <template slot="title">
                <i class="el-icon-s-home"></i>
                <span>首页</span>
              </template>
            </el-menu-item>

            <el-menu-item index="2">   
              <template slot="title">
                <i class="el-icon-document"></i>
                <span>文档</span>
              </template>
            </el-menu-item>

            <el-menu-item index="3">  
              <template slot="title">
                <i class="el-icon-s-promotion"></i>
                <span>引导页</span>
              </template>
            </el-menu-item>      

            <el-submenu index="4">   
              <template slot="title">
                <i class="el-icon-lock"></i>
                <span>权限测试页</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="4-1">页面权限</el-menu-item>
                <el-menu-item index="4-2">指令权限</el-menu-item>
                <el-menu-item index="4-3">角色权限</el-menu-item>
              </el-menu-item-group>
            </el-submenu>   

            <el-menu-item index="5">  
              <template slot="title">
                <i class="el-icon-picture"></i>
                <span>图标</span>
              </template>
            </el-menu-item>  

            <el-submenu index="6">   
              <template slot="title">
                <i class="el-icon-menu"></i>
                <span>组件</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="6-1">富文本编辑器</el-menu-item>                       
                <el-menu-item index="6-2">Markdown</el-menu-item>
                <el-menu-item index="6-3">JSON编辑器</el-menu-item>     
                <el-menu-item index="6-4">Splitpane</el-menu-item>
                <el-menu-item index="6-5">头像上传</el-menu-item>
                <el-menu-item index="6-6">Dropzone</el-menu-item>
              </el-menu-item-group>
            </el-submenu>

            <el-submenu index="7">  
              <template slot="title">
                <i class="el-icon-s-data"></i>
                <span>图表</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="7-1">键盘图表</el-menu-item>
                <el-menu-item index="7-2">折线图</el-menu-item>
                <el-menu-item index="7-3">混合图表</el-menu-item>     
              </el-menu-item-group>
            </el-submenu>

            <el-submenu index="8"> 
              <template slot="title">
                <i class="el-icon-s-flag"></i>
                <span>路由嵌套</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="8-1">菜单1</el-menu-item>
                <el-menu-item index="8-2">菜单2</el-menu-item>    
              </el-menu-item-group>
            </el-submenu>

            <el-submenu index="9">  
              <template slot="title">
                <i class="el-icon-film"></i>
                <span>Table</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="9-1">动态Table</el-menu-item>
                <el-menu-item index="9-2">拖拽Table</el-menu-item>
                <el-menu-item index="9-3">Table内编辑</el-menu-item>
                <el-menu-item index="9-4">综合Table</el-menu-item>    
              </el-menu-item-group>
            </el-submenu>

            <el-submenu index="10"> 
              <template slot="title">
                <i class="el-icon-s-help"></i>
                <span>综合实例</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="10-1">创建文章</el-menu-item>
                <el-menu-item index="10-2">文章列表</el-menu-item>    
              </el-menu-item-group>
            </el-submenu>

            <el-menu-item index="11"> 
              <template slot="title">
                <i class="el-icon-s-order"></i>
                <span>Tab</span>
              </template>
            </el-menu-item>

            <el-submenu index="12">  
              <template slot="title">
                <i class="el-icon-close"></i>
                <span>错误页面</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="12-1">401</el-menu-item>
                <el-menu-item index="12-2">404</el-menu-item>   
              </el-menu-item-group>
            </el-submenu>

            <el-menu-item index="13">  
              <template slot="title">
                <i class="el-icon-circle-close"></i>
                <span>错误日志</span>
              </template>
            </el-menu-item>

            <el-submenu index="14">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>Excel</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="14-1">导出 Excel</el-menu-item>
                <el-menu-item index="14-2">导出 已选择项</el-menu-item>   
                <el-menu-item index="14-3">导出 多级表头</el-menu-item>
                <el-menu-item index="14-4">上传 Excel</el-menu-item>
              </el-menu-item-group>
            </el-submenu>

            <el-submenu index="15">
              <template slot="title">
                <i class="el-icon-folder"></i>
                <span>Zip</span>
              </template>
              <el-menu-item-group>       
                <el-menu-item index="15-1">Export Zip</el-menu-item>
              </el-menu-item-group>
            </el-submenu>

            <el-menu-item index="16">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>PDF</span>
              </template>
            </el-menu-item>

            <el-menu-item index="17">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>换肤</span>
              </template>
            </el-menu-item>

            <el-menu-item index="18">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>Clipboard</span>
              </template>
            </el-menu-item>

            <el-menu-item index="19">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>国际化</span>
              </template> 
            </el-menu-item>

            <el-menu-item index="20">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>外链</span>
              </template>
            </el-menu-item>

            <el-menu-item index="21">
              <template slot="title">
                <i class="el-icon-tickets"></i>
                <span>打赏</span>
              </template>
            </el-menu-item>

          </el-menu>
        </el-col>
      </el-row>
    </div>

    <div id="right">
        <div id="right_1">

          <div id="right_2">
             <a href="http://www.baidu.com">
             <i class="el-icon-s-fold" style="font-size: 25px">
             </i>
             </a>
          </div>

           <el-breadcrumb-item><a href="/">&nbsp;&nbsp;&nbsp;&nbsp;首页&nbsp;&nbsp;&nbsp;/</a></el-breadcrumb-item>
           <el-breadcrumb-item><a href="/">Table &nbsp;&nbsp;/</a></el-breadcrumb-item>
           <el-breadcrumb-item><a href="/">综合Table</a></el-breadcrumb-item>

          <div id="right_3">  <!--右上方组件-->

               <a href="http://www.baidu.com">
                <el-tooltip content="搜索" placement="top">
               <i class="el-icon-search" 
                  style="font-size: 25px">
               </i>
               </el-tooltip>
               </a>&nbsp;&nbsp;

               <a href="http://www.baidu.com">
               <el-tooltip content="全屏" placement="top">
               <i class="el-icon-full-screen"
                  style="font-size: 25px">
               </i>
               </el-tooltip>
               </a>&nbsp;&nbsp;

               <a href="http://www.baidu.com">
               <el-tooltip content="布局大小" placement="top">
               <i class="el-icon-edit-outline" 
                  style="font-size:25px">
               </i>
               </el-tooltip>
               </a>&nbsp;&nbsp;

               <a href="http://www.baidu.com">
               <i class="el-icon-star-on" 
                  style="font-size: 25px">
               </i>
               </a>&nbsp;&nbsp;&nbsp;&nbsp;

               <a href="http://www.baidu.com"><el-tooltip content="个人中心" placement="top"><img src='./assets/1.gif' width="40px" height="40px" top="20px"></el-tooltip></a>
          </div>

        </div><br><br>

        <el-row>
           <el-button size=small>首页</el-button>
           <el-button size=small>文档</el-button>
           <el-tag :key="tag" closable :disable-transitions="false" @close="handleClose(tag)">综合Table</el-tag>
        </el-row><br>

       <el-input style="width:20%" v-model="input" placeholder="标题"></el-input> <!--输入框-->

       <el-select v-model="import" placeholder="重要性" style="width:10%"><!--重要性选择-->
           <el-option label="1" value="1"></el-option>
           <el-option label="2" value="2"></el-option>
           <el-option label="3" value="3"></el-option>
       </el-select>

       <el-select v-model="country" placeholder="类型" style="width:15%"><!--类型选择-->
           <el-option label="China" value="China(CN)"></el-option>
           <el-option label="USA" value="USA"></el-option>
           <el-option label="Japan" value="Japan"></el-option>
           <el-option label="Eurozone" value="Eurozone"></el-option>
       </el-select>

       <el-select v-model="ID" placeholder="ID Ascending" style="width:15%"><!--ID选择-->
           <el-option label="ID Ascending" value="ID Ascending"></el-option>
           <el-option label="ID Dscending" value="ID Dscending"></el-option>
       </el-select>
       <template slot-scope="scope">
       <el-button type="primary" icon="el-icon-search" style="width:8%" @click="searchHandler(scope.$index, scope.rowData)">搜索</el-button>
       </template>
       <el-button type="primary" icon="el-icon-edit" style="width:8%" @click="dialogFormVisible = true">添加</el-button><!--添加表单-->
            <el-dialog title="Edit" :visible.sync="dialogFormVisible">
              <el-form :model="form">

                 <el-form-item label="类型" :label-width="formLabelWidth">
                      <el-select v-model="form.country" placeholder="Japan">
                        <el-option label="China" value="China"></el-option>
                        <el-option label="USA" value="USA"></el-option>
                        <el-option label="Japan" value="Japan"></el-option>
                        <el-option label="Eurozone" value="Eurozone"></el-option>
                     </el-select>
                 </el-form-item>

                 <el-form-item label="时间" :label-width="formLabelWidth">
                        <el-date-picker v-model="form.time" type="datetime" placeholder="选择日期时间">
                        </el-date-picker>
                 </el-form-item>

                 <el-form-item label="标题" :label-width="formLabelWidth">
                        <el-input v-model="form.title" autocomplete="off">
                        </el-input>
                 </el-form-item>

                 <el-form-item label="状态" :label-width="formLabelWidth">
                    <el-select v-model="form.tag" placeholder="draft">
                        <el-option label="draft" value="draft"></el-option>
                        <el-option label="published" value="published"></el-option>
                        <el-option label="deleted" value="deleted"></el-option>
                    </el-select>
                 </el-form-item>

                 <el-form-item label="评分" :label-width="formLabelWidth">
                     <el-rate v-model="form.import">
                     </el-rate>
                 </el-form-item>
        
                 <el-form-item label="点评" :label-width="formLabelWidth">
                     <el-input type="textarea" :rows="2" placeholder="please input" v-model="textarea">
                     </el-input>
                 </el-form-item>

              </el-form>

              <div slot="footer" class="dialog-footer">
                 <el-button @click="dialogFormVisible = false">取 消</el-button>
                 <el-button type="primary" @click="handleFormSave">确 定</el-button>
              </div>
            </el-dialog>
          &nbsp;&nbsp;
           <el-button type="primary" icon="el-icon-download" style="width:8%">导出</el-button>
           <el-checkbox v-model="checked" style="width:1%">审核人</el-checkbox>


            <el-dialog title="Readingstatistics" :visible.sync="dialogVisible">
                 <table  
                 style='width: 700px;
                 height:300px;
                 border: 1px solid #dfe6ec;'
                 border="0" 
                 cellpadding="0" 
                 cellspacing="0"> 
                    <tr>
                        <th rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">Channel</th> 
                         <th owspan='1' colspan="1"style="border: 1px solid #dfe6ec;">Pv</th>
                    </tr>
                    <tr>
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">PC</td> 
                         <td owspan='1' colspan="1"style="border: 1px solid #dfe6ec;">1024</td>
                    </tr>
                    <tr>
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">mobile</td>  
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">1024</td>   
                    </tr>
                    <tr>
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">ios</td>  
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">1024</td>   
                    </tr>
                    <tr>
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">android</td>  
                        <td rowspan='1' colspan="1"style="border: 1px solid #dfe6ec;">1024</td>   
                    </tr>
                 </table>
                  <div slot="footer" class="dialog-footer">
                      <el-button type="primary" @click="dialogVisible = false">确 定</el-button>
                  </div>
            </el-dialog>
    </div>


    <div id="main"><!-- 表格内数据 -->
       <el-table :data="tableData" border style="width:98%">
          <el-table-column
            prop="xh"
            label="序号"
            width="50">
          </el-table-column>

          <el-table-column
            prop="time"
            label="时间"
            width="150">
          </el-table-column>

          <el-table-column
            prop="title"
            label="标题"
            width="420"
            style="text-align: center;">
            <template slot-scope="scope">
             <el-button type="text" style="width:8%" :title="scope.row.title" @click="handleEdit(scope.$index, scope.row)">{{scope.row.title}}</el-button>
             <br>
              <el-tag
                :type="tag"
                disable-transitions>{{scope.row.country}}
              </el-tag>
            </template>
          </el-table-column>

          <el-table-column
            prop="author"
            label="作者"
            width="95">
          </el-table-column>

          <el-table-column
            prop="import"
            label="重要性"
            width="80">
          </el-table-column>

          <el-table-column
            prop="read"
            label="阅读数"
            width="80">
            <template slot-scope='scope'>
                             <el-button type='text' :read="scope.row.read" @click="dialogVisible = true">      
                                <span style="color:#338dd0">{{scope.row.read}}</span>
                            </el-button>
                        </template>
          </el-table-column>

          <el-table-column
            prop="tag"
            label="状态"
            width="100"
            :filters="[{ text: 'published', value: 'published' }, { text: 'draft', value: 'draft' }]"
            :filter-method="filterTag"
            filter-placement="bottom-end"> 
            <template slot-scope="scope">
              <el-tag
                :type="scope.row.tag === 'published' ? 'success' : 'info'"
                disable-transitions>{{scope.row.tag}}
              </el-tag>
            </template>
          </el-table-column>

          <el-table-column prop="operate" label="操作" width='248'
                        :filters="[{ text: '草稿', value: '草稿' }, { text: '发布', value: '发布' }]"
                        :filter-method="filteroperate"
                        filter-placement="bottom-end">
                                <template slot-scope="scope">
                                 <center>
                                    <el-button  type="primary" size="small" @click="handleEdit(scope.$index, scope.row)">编辑</el-button>
                                    <el-button  size="small" :type="scope.row.tag === 'published' ? '' : 'success'" @click='open2(scope.$index, scope.row)' disable-transitions>{{scope.row.operate}}</el-button>
                                    <el-button size="small" type="danger" @click.native.prevent="handleDelete(scope.$index, tableData)">删除</el-button>
                                  </center>
                                </template>
          </el-table-column>

        </el-table>
       <br><br><br>
         
        <div id="block">   <!-- 底部导航 -->
             <el-pagination
                  @size-change="handleSizeChange"
                  @current-change="handleCurrentChange"
                  :current-page="currentPage4"
                  :page-sizes="[10, 20, 30, 40,50]"
                  :page-size="20"
                  layout="total, sizes, prev, pager, next, jumper"
                  :total="100">
             </el-pagination>
             <br><br><br>
        </div>
    </div>
    
  </div>
</template>

<script>
export default 
{
  name: 'App',
  data() {
      return {
       tableData: 
      [ 
         {
          xh:'1',
          time:'2011-04-11 23:15',
          title:'Irlbxqd Kbxhn Yjnhof Fbclrk Ngfyiii Dqslf Kqijhdi Pxltw Xdqse',
          author:'Robert',
          import:'⭐⭐',
          read:'798',
          tag:'published',
          country:'USA',
          operate:'草稿'
         }, 
         {
          xh:'2',
          time:'2019-08-05 05:33',
          title:'Ffqnqwlr Ljqtw Nivoda Pcfeeb Gcsyddqd',
          author:'Nancy',
          import:'⭐⭐⭐',
          read:'4023',
          tag:'published',
          country:'USA',
          operate:'草稿'
         }, 
         {
          xh:'3',
          time:'2014-07-30 23:48',
          title:'Hrhu Rdvjask Axe Alq Odls Eua Xekcixll Hygbse',
          author:'Lisa',
          import:'⭐',
          read:'1178',
          tag:'published',
          country:'USA',
          operate:'草稿'      
         }, 
         {
          xh:'4',
          time:'1997-08-28 23:07',
          title:'Mmafxlss Pnvghsuwu Olyqbr Gkmfxoyaoj Xetnecbpk Tetktsvhk',
          author:'Donald',
          import:'⭐⭐',
          read:'3850',
          tag:'published',
          country:'Eurozone',
          operate:'草稿'
         },
         {
          xh:'5',
          time:'1974-10-26 02:16',
          title:'Qutvjwm Svnpycountryagk Rxzb Vwmlj Rjs Akgeotcgvf Mzscyegqiu',
          author:'Brian',
          import:'⭐',
          read:'7645',
          tag:'published',
          country:'Japan',
          operate:'草稿'
         },
         {
          xh:'6',
          time:'1971-10-28 19:35',
          title:'Mjctxtxlfv Gnnrmp Jsk Hczj Npnyrb Lxnyigrghk Kgjf Vgwhxdd',
          author:'Kimberly',
          import:'⭐⭐',
          read:'1279',
          tag:'published',
          country:'China',
          operate:'草稿'
         },
         {
          xh:'7',
          time:'2010-09-10 02:51',
          title:'Rdpzbdpm Lbfjgoe Dwjyfvf Mynx Lpxw',
          author:'Ruth',
          import:'⭐⭐',
          read:'2375',
          tag:'published',
          country:'USA',
          operate:'草稿'
         },
         {
          xh:'8',
          time:'2011-04-11 23:15',
          title:'Fivbjduf Jfgpuitlm Lgyzs Igrchgxw Etdbhv Dmkklvae',
          author:'Jessica',
          import:'⭐',
          read:'4959',
          tag:'published',
          country:'Eurozone',
          operate:'草稿'
         },
         {
          xh:'9',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐',
          read:'1862',
          tag:'published',
          country:'USA',
          operate:'草稿'
         },
         {
          xh:'10',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐',
          read:'1862',
          tag:'published',
          country:'Japan',
          operate:'草稿'
         },
         {
          xh:'11',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐',
          read:'1862',
          tag:'published',
          country:'USA',
          operate:'草稿'
         },
         {
          xh:'12',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐',
          read:'1862',
          tag:'published',
          country:'China',
          operate:'草稿'
         },
         {
          xh:'13',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐⭐',
          read:'1862',
          tag:'published',
          country:'China',
          operate:'草稿'
         },
         {
          xh:'14',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐⭐',
          read:'1862',
          tag:'published',
          country:'USA',
          operate:'草稿'
         },
         {
          xh:'15',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐',
          read:'1862',
          tag:'published',
          country:'Eurozone',
          operate:'草稿'
         },
         {
          xh:'16',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐',
          read:'1862',
          tag:'published',
          country:'USA',
          operate:'草稿'
         },
         {
          xh:'17',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐',
          read:'1862',
          tag:'published',
          country:'China',
          operate:'草稿'
         },
         {
          xh:'18',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐',
          read:'1862',
          tag:'published',
          country:'Japan',
          operate:'草稿'
         },
         {
          xh:'19',
          time:'2011-04-11 23:15',
          title:'Tlmooo Chjnor Rjep Fbdclrpnb Fsylygq Vzoglrlu',
          author:'Donald',
          import:'⭐⭐⭐',
          read:'1862',
          tag:'published',
          country:'USA',
          operate:'草稿'
         },
      ],
         textarea: '',
         dialogVisible:false,
         dialogTableVisible: false,
         dialogFormVisible: false,
         count:0,
         //表单内数据
         form: 
         {
             time:'',
             title: '',
             country:'',
             tag:'', 
             import:'',
             date1: '',
             date2: '',
             delivery: false,
             type: [],
             resource: '',
             desc: ''
            
         },
        formLabelWidth: '120px',
        checked: false,
        input: '',
      };
    },
  methods: 
  {
    //标签页
    handleClose(tag)
    {
        this.dynamicTags.splice(this.dynamicTags.indexOf(tag), 1);
    },
    //底部页面跳转
    handleSizeChange(val)
    {
        console.log(`每页 ${val} 条`);
    },
    handleCurrentChange(val)
    {
        console.log(`当前页: ${val}`);
    },
    //打开菜单下拉框
    handleOpen(key, keyPath) 
    {  
        console.log(key, keyPath);
    },
    handleClose(key, keyPath)
    {
        console.log(key, keyPath);
    },
    //删除按钮
    handleFormSave() 
    {
         this.$notify
         ({
                title: '成功',
                message: '更新成功',
                type: 'success'
         });
         this.tableData[this.form.xh - (this.count+1)].title = this.form.title;
         this.tableData[this.form.xh - (this.count+1)].time =this.form.time;
         this.tableData[this.form.xh - (this.count+1)].tag = this.form.tag;
         this.tableData[this.form.xh - (this.count+1)].country = this.form.country;
          if(this.tableData[this.form.xh - (this.count+1)].tag ==='draft')
          {
              console.log(this.tableData[this.form.xh - (this.count+1)].operate='发布') 
          }
          else
          {
              console.log(this.tableData[this.form.xh - (this.count+1)].operate='草稿') 
          }
          this.dialogFormVisible = false;
          console.log(this.count);
    },

    handleEdit(index, rowData) 
    {
            console.log(index, rowData);
            this.form.title = rowData.title;
            this.form.time = rowData.time;
            this.form.country = rowData.country;
            this.form.tag = rowData.tag;
            this.form.import = rowData.import;
            this.form.xh=rowData.xh;
            this.form.operate=rowData.operate;
            this.dialogFormVisible = true;
    },
    //按钮与
    open2(index,row) 
    {
            this.$message({
              message: '操作成功',
              type: 'success',
            });
            this.tableData[index].operate=row.operate;
            if(this.tableData[index].operate ==="发布"){
              console.log(this.tableData[index].operate='草稿');
              console.log(this.tableData[index].tag='published');
            }else{
              console.log(this.tableData[index].operate='发布');
              console.log(this.tableData[index].tag='draft');
          }
    },
      //删除信息
    handleDelete(index,row)
    {
            this.count++;
            row.splice(index,1);
            console.log(this.count)
    },

    searchHandler(index,rowData)
    {
    
       if (this.country.value === this.tableData[this.form.xh - (this.count+1)].country)
         console.log(index,rowData);
    }
  }
}
</script>

<style>
    #app 
    {
      font-family: 'Avenir', Helvetica, Arial, sans-serif;
      -webkit-font-smoothing: antialiased;
      -moz-osx-font-smoothing: grayscale;
      text-align: left;
      color: #2c3e50;
      height:100vh;
      margin:0px;
    }

    #left
    {
      float:left;
      width:19%;
      height:100vh;
      margin: 0px;
      left: 0;
      bottom: 0;
      overflow-x:hidden;
      position: fixed;
      overflow-y:scroll;
       &::-webkit-scrollbar {
        display: none;
      } 

    }

    #right
    {
      padding-left: 10px;
      width:79%;
      height:150px;
      float:right;
    }

    #right_2
    {

      float: left;
    }

    #right_3{

      float: right;
    }

    #main{
      width:80%;
      height:100vh;
      float:right;
      text-align: center;
      padding-left:12px;
    }

    #block{
      float: left;
      height: 50px;
    }

</style> 