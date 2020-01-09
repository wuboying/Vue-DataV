<template>
	<div id="home">
		<dv-full-screen-container>
			<top-header />
			<div class="main-content">
				<digital-flop />
				<div class="block-left-right-content">
					<ranking-board />
					<div class="block-top-bottom-content">
						<div class="block-top-content">
							<rose-chart />

							<water-level-chart />

							<scroll-board />
						</div>
						<div class="block-bottom-content">
							
						 <cards />
						</div>
					</div>
				</div>
			</div>
		</dv-full-screen-container>
	</div>
</template>

<script>
import topHeader from '../components/topHeader.vue';
import digitalFlop from '../components/digitalFlop.vue';
import rankingBoard from '../components/rankingBoard.vue';
import roseChart from '../components/roseChart.vue';
import waterLevelChart from '../components/waterLevelChart.vue';
import scrollBoard from '../components/scrollBoard.vue';
import cards from '../components/cards.vue'

export default {
	name: 'home',
	components: {
		topHeader,
		digitalFlop,
		rankingBoard,
		roseChart,
		waterLevelChart,
		scrollBoard,
		cards
	}
};
</script>
<style lang="scss">
#home {
	width: 100%;
	height: 100%;
	background-color: #030409;
	color: #fff;
	#dv-full-screen-container {
		width: 100%;
		height: 100%;
		background-image: url('../assets/img/bg.png');
		background-size: 100% 100%;
		box-shadow: 0 0 3px blue;
		display: flex;
		flex-direction: column;
	}
	.main-content {
		flex: 1;
		display: flex;
		flex-direction: column;
	}
	.block-left-right-content {
		flex: 1;
		display: flex;
		margin-top: 20px;
	}
	.block-top-bottom-content {
		flex: 1;
		display: flex;
		flex-direction: column;
		box-sizing: border-box;
		padding-left: 20px;
	}
	.block-top-content {
		height: 55%;
		display: flex;
		flex-grow: 0;
		box-sizing: border-box;
		padding-bottom: 20px;
	}
	.block-bottom-content {
		height: 45%;
		display: flex;
		flex-grow: 0;
		box-sizing: border-box;
	}
}
</style>
