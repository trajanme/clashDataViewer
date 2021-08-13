<template>
  <v-row justify="center" align="center">
    <v-col cols="12" sm="8" md="6">
      <v-list subheader>
      <v-subheader>エリクサーユニット</v-subheader>

      <v-list-item　v-for="chat in elixirUnit" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>

        <!-- <v-list-item-action>
          <v-btn icon>
            <v-icon color="grey lighten-1">mdi-information</v-icon>
          </v-btn>
        </v-list-item-action> -->
      </v-list-item>
    </v-list>
    
    <v-divider></v-divider>

    <v-list subheader>
    <v-subheader>ダークエリクサーユニット</v-subheader>

      <v-list-item　v-for="chat in darkElixirUnit" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>

    </v-list>

    <v-divider></v-divider>

    <v-list subheader>
    <v-subheader>スーパーユニット</v-subheader>

      <v-list-item　v-for="chat in superUnit" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>

    </v-list>

    <v-divider></v-divider>

    <v-list subheader>
    <v-subheader>呪文</v-subheader>

      <v-list-item　v-for="chat in spell" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>

    </v-list>

    <v-divider></v-divider>

    <v-list subheader>
    <v-subheader>闇の呪文</v-subheader>

      <v-list-item　v-for="chat in darkSpell" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>

    </v-list>

    <v-divider></v-divider>

    <v-list subheader>
    <v-subheader>突破兵器</v-subheader>

      <v-list-item　v-for="chat in weapons" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>

    </v-list>

    <v-divider></v-divider>

    <v-list subheader>
    <v-subheader>ヒーロー</v-subheader>

      <v-list-item　v-for="chat in hero" :key="chat.title">
        <v-list-item-avatar>
          <v-img
            :alt="`${chat.title} avatar`"
            :src="chat.avatar"
          ></v-img>
        </v-list-item-avatar>

        <v-list-item-content>
          <v-list-item-title v-text="chat.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>

    </v-list>

    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    elixirUnit: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Barbarian.png?raw=true',
        title: 'バーバリアン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Archer.png?raw=true',
        title: 'アーチャー',
      },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Giant.png?raw=true',
          title: 'ジャイアント',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Goblin.png?raw=true',
          title: 'ゴブリン',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Wall_Breaker.png?raw=true',
          title: 'ウォールブレイカー',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Balloon.png?raw=true',
          title: 'バルーン',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Wizard.png?raw=true',
          title: 'ウィザード',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Healer.png?raw=true',
          title: 'ヒーラー',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Dragon.png?raw=true',
          title: 'ドラゴン',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/P.E.K.K.A.png?raw=true',
          title: 'P.E.K.K.A',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Baby_Dragon.png?raw=true',
          title: 'ベビードラゴン',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Miner.png?raw=true',
          title: 'ディガー',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Electro_Dragon.png?raw=true',
          title: 'ライトニングドラゴン',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Yeti.png?raw=true',
          title: 'イエティ',
        },
        {
          avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Dragon_Rider.png?raw=true',
          title: 'ドラゴンライダー',
        },
    ],
    darkElixirUnit: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Minion.png?raw=true',
        title: 'ガーゴイル',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Hog_Rider.png?raw=true',
        title: 'ホグライダー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Valkyrie.png?raw=true',
        title: 'バルキリー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Golem.png?raw=true',
        title: 'ゴーレム',
      },
            {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Witch.png?raw=true',
        title: 'ネクロマンサー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Lava_Hound.png?raw=true',
        title: 'ラヴァハウンド',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Bowler.png?raw=true',
        title: 'ボウラー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Ice_Golem.png?raw=true',
        title: 'アイスゴーレム',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Headhunter.png?raw=true',
        title: 'ストライカー',
      },
    ],
    superUnit: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Barbarian.png?raw=true',
        title: 'スーパーバーバリアン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Archer.png?raw=true',
        title: 'スーパーアーチャー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Giant.png?raw=true',
        title: 'スーパージャイアント',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Sneaky_Goblin.png?raw=true',
        title: 'スニークゴブリン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Wall_Breaker.png?raw=true',
        title: 'スーパーウォールブレイカー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Rocket_Balloon.png?raw=true',
        title: 'ロケットバルーン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Wizard.png?raw=true',
        title: 'スーパーウィザード',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Inferno_Dragon.png?raw=true',
        title: 'インフェルノドラゴン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Minion.png?raw=true',
        title: 'スーパーガーゴイル',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Valkyrie.png?raw=true',
        title: 'スーパーバルキリー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Super_Witch.png?raw=true',
        title: 'スーパーネクロマンサー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Ice_Hound.png?raw=true',
        title: 'アイスハウンド',
      }
    ],
    spell: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Lightning_Spell.png?raw=true',
        title: 'ライトニングの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Healing_Spell.png?raw=true',
        title: 'ヒールの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Rage_Spell.png?raw=true',
        title: 'レイジの呪文',
      },
            {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Jump_Spell.png?raw=true',
        title: 'ジャンプの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Freeze_Spell.png?raw=true',
        title: 'フリーズの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Clone_Spell.png?raw=true',
        title: 'クローンの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Invisibility_Spell.png?raw=true',
        title: 'インビジブルの呪文',
      },
    ],
    darkSpell: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Poison_Spell.png?raw=true',
        title: 'ポイズンの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Earthquake_Spell.png?raw=true',
        title: 'アースクエイクの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Haste_Spell.png?raw=true',
        title: 'ヘイストの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Skeleton_Spell.png?raw=true',
        title: 'スケルトンの呪文',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Bat_Spell.png?raw=true',
        title: 'コウモリの呪文',
      },
    ],
    weapons: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Wall_Wrecker.png?raw=true',
        title: 'ウォールバスター',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Battle_Blimp.png?raw=true',
        title: '突撃艦',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Stone_Slammer.png?raw=true',
        title: 'ロックボマー',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Siege_Barracks.png?raw=true',
        title: '投下兵舎',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Log_Launcher.png?raw=true',
        title: 'ウッドランチャー',
      },
    ],
    hero: [
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Barbarian_King.png?raw=true',
        title: 'バーバリアンキング',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Archer_Queen.png?raw=true',
        title: 'アーチャークイーン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Grand_Warden.png?raw=true',
        title: 'グランドウォーデン',
      },
      {
        avatar: 'https://github.com/Statscell/clash-assets/blob/main/troops/icons/Royal_Champion.png?raw=true',
        title: 'ロイヤルチャンピオン',
      },
    ],
  })
}
</script>
