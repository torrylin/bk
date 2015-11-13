<script>
	module.exports = {
		data: function () {
			var states = [
				{ name: 'Alabama', num: 0 },
				{ name: 'Arizona', num: 1 },
				{ name: 'California', num: 2 },
				{ name: 'Alaska', num: 3 }
			];
			return {
				states: states
			}
		},

	}
</script>

<template>
	<div class="bk-home-newClient">
		<div class="panel panel-default">
			<div class="panel-heading">New Client</div>
			<div class="panel-body">
				<div class="col-md-3 bk-input-padding">
					<input type="text" placeholder="First Name" class="form-control">
				</div>
				<div class="col-md-2 bk-input-padding">
					<input type="text" placeholder="M Name" class="form-control">
				</div>
				<div class="col-md-3 bk-input-padding">
					<input type="text" placeholder="Last Name" class="form-control">
				</div>
				<div class="col-md-3 bk-input-padding">
					<select class="form-control">
						<template v-for="state in states">
							<option value="{{state.num}}">{{state.name}}</option>
						</template>
					</select>
				</div>
				<div class="col-md-1 bk-input-padding">
					<button class="btn btn-default">Next</button>
				</div>
			</div>
		</div>
	</div>
</template>

<style>
	.bk-home-newClient {
		width: 650px;
	}
	.bk-home-newClient .bk-input-padding {
		padding: 2px;
	}
</style>