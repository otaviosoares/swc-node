# Snapshot report for `packages/jest/__test__/hoist-top-level.spec.ts`

The actual snapshot is saved in `hoist-top-level.spec.ts.snap`.

Generated by [AVA](https://avajs.dev).

## should hoist top level jest mock call

> Snapshot 1

    `"use strict";␊
    jest.enableAutomock();␊
    jest.disableAutomock();␊
    jest.mock('./foo');␊
    jest.mock('./foo/bar', ()=>'bar');␊
    jest.deepUnmock('./foo');␊
    jest.mock('./foo').mock('./bar');␊
    const foo = 'foo';␊
    console.log(foo);␊
    jest.unmock('./bar/foo').dontMock('./bar/bar');␊
    const func = ()=>{␊
        jest.unmock('./foo');␊
        jest.mock('./bar');␊
        jest.mock('./bar/foo', ()=>'foo');␊
        jest.unmock('./foo/bar');␊
        jest.deepUnmock('./bar');␊
        jest.mock('./foo').mock('./bar');␊
        const bar = 'bar';␊
        console.log(bar);␊
        jest.unmock('./bar/foo').dontMock('./bar/bar');␊
    };␊
    const func2 = ()=>{␊
        jest.mock('./bar');␊
        jest.unmock('./foo/bar');␊
        jest.mock('./bar/foo', ()=>'foo');␊
        jest.unmock('./foo');␊
        jest.deepUnmock('./bar');␊
        jest.mock('./foo').mock('./bar');␊
        const bar = 'bar';␊
        console.log(bar);␊
        jest.unmock('./bar/foo').dontMock('./bar/bar');␊
    };␊
    ␊
    //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJzb3VyY2VzIjpbImplc3Quc3BlYy50cyJdLCJzb3VyY2VzQ29udGVudCI6WyJcbmNvbnN0IGZvbyA9ICdmb28nXG5jb25zb2xlLmxvZyhmb28pXG5qZXN0LmVuYWJsZUF1dG9tb2NrKClcbmplc3QuZGlzYWJsZUF1dG9tb2NrKClcbmplc3QubW9jaygnLi9mb28nKVxuamVzdC5tb2NrKCcuL2Zvby9iYXInLCAoKSA9PiAnYmFyJylcbmplc3QudW5tb2NrKCcuL2Jhci9mb28nKS5kb250TW9jaygnLi9iYXIvYmFyJylcbmplc3QuZGVlcFVubW9jaygnLi9mb28nKVxuamVzdC5tb2NrKCcuL2ZvbycpLm1vY2soJy4vYmFyJylcbmNvbnN0IGZ1bmMgPSAoKSA9PiB7XG4gIGNvbnN0IGJhciA9ICdiYXInXG4gIGNvbnNvbGUubG9nKGJhcilcbiAgamVzdC51bm1vY2soJy4vZm9vJylcbiAgamVzdC5tb2NrKCcuL2JhcicpXG4gIGplc3QubW9jaygnLi9iYXIvZm9vJywgKCkgPT4gJ2ZvbycpXG4gIGplc3QudW5tb2NrKCcuL2Zvby9iYXInKVxuICBqZXN0LnVubW9jaygnLi9iYXIvZm9vJykuZG9udE1vY2soJy4vYmFyL2JhcicpXG4gIGplc3QuZGVlcFVubW9jaygnLi9iYXInKVxuICBqZXN0Lm1vY2soJy4vZm9vJykubW9jaygnLi9iYXInKVxufVxuY29uc3QgZnVuYzIgPSAoKSA9PiB7XG4gIGNvbnN0IGJhciA9ICdiYXInXG4gIGNvbnNvbGUubG9nKGJhcilcbiAgamVzdC5tb2NrKCcuL2JhcicpXG4gIGplc3QudW5tb2NrKCcuL2Zvby9iYXInKVxuICBqZXN0Lm1vY2soJy4vYmFyL2ZvbycsICgpID0+ICdmb28nKVxuICBqZXN0LnVubW9jaygnLi9mb28nKVxuICBqZXN0LnVubW9jaygnLi9iYXIvZm9vJykuZG9udE1vY2soJy4vYmFyL2JhcicpXG4gIGplc3QuZGVlcFVubW9jaygnLi9iYXInKVxuICBqZXN0Lm1vY2soJy4vZm9vJykubW9jaygnLi9iYXInKVxufVxuIl0sIm5hbWVzIjpbImplc3QiLCJlbmFibGVBdXRvbW9jayIsImRpc2FibGVBdXRvbW9jayIsIm1vY2siLCJkZWVwVW5tb2NrIiwiZm9vIiwiY29uc29sZSIsImxvZyIsInVubW9jayIsImRvbnRNb2NrIiwiZnVuYyIsImJhciIsImZ1bmMyIl0sIm1hcHBpbmdzIjoiO0FBR0FBLEtBQUtDLGNBQWM7QUFDbkJELEtBQUtFLGVBQWU7QUFDcEJGLEtBQUtHLElBQUksQ0FBQztBQUNWSCxLQUFLRyxJQUFJLENBQUMsYUFBYSxJQUFNO0FBRTdCSCxLQUFLSSxVQUFVLENBQUM7QUFDaEJKLEtBQUtHLElBQUksQ0FBQyxTQUFTQSxJQUFJLENBQUM7QUFSeEIsTUFBTUUsTUFBTTtBQUNaQyxRQUFRQyxHQUFHLENBQUNGO0FBS1pMLEtBQUtRLE1BQU0sQ0FBQyxhQUFhQyxRQUFRLENBQUM7QUFHbEMsTUFBTUMsT0FBTyxJQUFNO0lBR2pCVixLQUFLUSxNQUFNLENBQUM7SUFDWlIsS0FBS0csSUFBSSxDQUFDO0lBQ1ZILEtBQUtHLElBQUksQ0FBQyxhQUFhLElBQU07SUFDN0JILEtBQUtRLE1BQU0sQ0FBQztJQUVaUixLQUFLSSxVQUFVLENBQUM7SUFDaEJKLEtBQUtHLElBQUksQ0FBQyxTQUFTQSxJQUFJLENBQUM7SUFSeEIsTUFBTVEsTUFBTTtJQUNaTCxRQUFRQyxHQUFHLENBQUNJO0lBS1pYLEtBQUtRLE1BQU0sQ0FBQyxhQUFhQyxRQUFRLENBQUM7QUFHcEM7QUFDQSxNQUFNRyxRQUFRLElBQU07SUFHbEJaLEtBQUtHLElBQUksQ0FBQztJQUNWSCxLQUFLUSxNQUFNLENBQUM7SUFDWlIsS0FBS0csSUFBSSxDQUFDLGFBQWEsSUFBTTtJQUM3QkgsS0FBS1EsTUFBTSxDQUFDO0lBRVpSLEtBQUtJLFVBQVUsQ0FBQztJQUNoQkosS0FBS0csSUFBSSxDQUFDLFNBQVNBLElBQUksQ0FBQztJQVJ4QixNQUFNUSxNQUFNO0lBQ1pMLFFBQVFDLEdBQUcsQ0FBQ0k7SUFLWlgsS0FBS1EsTUFBTSxDQUFDLGFBQWFDLFFBQVEsQ0FBQztBQUdwQyJ9`
