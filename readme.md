# Ferramentas

    *mocha* - test runner
    *chai* - lib de assertions
    *istambul* - lib de coverage
    *sinon* - lib de mocks, spies e stubs

    spies = verifica se função original foi chamada mas não interfere na execução
    stubs = são spies com comportamento pré-programado, podendo interferir na execução

## Estrutura exemplo de um test

```js
describe("Main", () => {
  describe("Método A", () => {
    it("Should return 1", () => {
      throw new Error("só um erro aí");
    });
  });
});
```

## Exemplo de comando de execução

npm run test -- --bail --reporter=progress

```js
"scripts": {
    "test": "npx mocha tests/**/*.spec.js"
  },
```

## Lista de opções para o comando mocha
--bail = Falha no primeiro test
--reporter = set reporter que vai ser utilizado
--reporters = get lista de reporters disponíveis
--watch = 

## Lista de hooks
before() = roda uma vez antes do bloco
after() = roda uma vez depois do bloco
beforeEach() = roda antes de todos bloco
afterEach() = roda depois de cada bloco


## Conceitos
Todo it retorna uma exception qndo falha
context.only() - roda somente context específico
context.skip() - skipa um context específico
hooks = código executado a partir de uma ação

### Smoke test
"SMOKE TESTING, also known as “Build Verification Testing”, is a type of software testing that comprises of a non-exhaustive set of tests that aim at ensuring that the most important functions work. The result of this testing is used to decide if a build is stable enough to proceed with further testing."
                                                                    - softwaretestingfundamentals.com › smoke-testing

