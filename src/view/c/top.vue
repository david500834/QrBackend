<template>
    
		<div class="col-md-12">
			<nav class="navbar navbar-default " role="navigation">
				<div class="navbar-header">
					 
					<button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1">
						 <span class="sr-only">Toggle navigation</span><span class="icon-bar"></span><span class="icon-bar"></span><span class="icon-bar"></span>
					</button> <router-link class="navbar-brand" :to="'/mall/'+loc_id+'/'">商城后台</router-link>
				</div>
				
				<div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1">
					<ul class="nav navbar-nav">
						<li >
							<router-link :to="'/mall/'+loc_id+'/'">商品</router-link>
						</li>
						<li >
							<router-link to="/order">订单</router-link>
						</li>
						
					</ul>
					
					<ul class="nav navbar-nav navbar-right">
						<li>
							<a>退出</a>
						</li>
<!--
						<li class="dropdown">
							 <a href="#" class="dropdown-toggle" data-toggle="dropdown">Dropdown<strong class="caret"></strong></a>
							<ul class="dropdown-menu">
								<li>
									<a href="#">Action</a>
								</li>
								<li>
									<a href="#">Another action</a>
								</li>
								<li>
									<a href="#">Something else here</a>
								</li>
								<li class="divider">
								</li>
								<li>
									<a href="#">Separated link</a>
								</li>
							</ul>
						</li>
-->
					</ul>
				</div>
				
			</nav>
		</div>

</template>
<script>
export default{
data(){
    return {
    loc_id:""
    }
},
    created(){
        let self = this
        self.loc_id = self.$route.params["loc_id"]
    
    }
}
</script> 
