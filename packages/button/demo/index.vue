<template>
  <demo-section>
    <demo-block :title="$t('type')">
      <div class="demo-button-row">
        <van-button type="primary">{{ $t('primary') }}</van-button>
        <van-button type="danger">{{ $t('danger') }}</van-button>
      </div>
      <van-button type="default">{{ $t('default') }}</van-button>
      <van-button type="warning">{{ $t('warning') }}</van-button>
    </demo-block>

    <demo-block :title="$t('plain')">
      <van-button
        plain
        type="primary"
      >
        {{ $t('plain') }}
      </van-button>
      <van-button
        plain
        type="danger"
      >
        {{ $t('plain') }}
      </van-button>
    </demo-block>

    <demo-block :title="$t('disabled')">
      <van-button
        disabled
        type="primary"
      >
        {{ $t('disabled') }}
      </van-button>
      <van-button
        disabled
        type="danger"
      >
        {{ $t('disabled') }}
      </van-button>
    </demo-block>

    <demo-block :title="$t('loading')">
      <van-button
        loading
        type="primary"
      />
      <van-button
        loading
        type="danger"
      />
    </demo-block>

    <demo-block :title="$t('shape')">
      <van-button
        type="primary"
        square
      >
        {{ $t('square') }}
      </van-button>
      <van-button
        type="danger"
        round
      >
        {{ $t('round') }}
      </van-button>
    </demo-block>

    <demo-block :title="$t('size')">
      <van-button size="large">{{ $t('large') }}</van-button>
      <van-button size="normal">{{ $t('normal') }}</van-button>
      <van-button size="small">{{ $t('small') }}</van-button>
      <van-button size="mini">{{ $t('mini') }}</van-button>
    </demo-block>
  </demo-section>
</template>

<script>
export default {
  i18n: {
    'zh-CN': {
      type: '按钮类型',
      size: '按钮尺寸',
      loading: '加载状态',
      shape: '按钮形状',
      default: '默认按钮',
      primary: '主要按钮',
      danger: '危险按钮',
      warning: '警告按钮',
      large: '大号按钮',
      normal: '普通按钮',
      small: '小型按钮',
      mini: '迷你按钮',
      plain: '朴素按钮',
      square: '方形按钮',
      round: '圆形按钮'
    },
    'en-US': {
      type: 'Type',
      size: 'Size',
      loading: 'Loading',
      shape: 'Shape',
      default: 'Default',
      primary: 'Primary',
      danger: 'Danger',
      warning: 'Warning',
      large: 'Large',
      normal: 'Normal',
      small: 'Small',
      mini: 'Mini',
      plain: 'Plain',
      square: 'Square',
      round: 'Round'
    }
  }
};
</script>

<style lang="less">
.demo-button {
  .van-button {
    user-select: none;

    &--large {
      margin-bottom: 15px;
    }

    &--small,
    &--normal:not(:last-child) {
      margin-right: 10px;
    }

    .van-loading {
      margin: 0 18px;
    }
  }

  .van-doc-demo-block {
    padding: 0 15px;
  }

  .van-doc-demo-block__title {
    padding-left: 0;
  }

  &-row {
    margin-bottom: 10px;
  }
}
</style>
