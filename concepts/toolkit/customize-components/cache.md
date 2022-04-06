---
title: Microsoft Graph Toolkit cache
description: Explicando como o Cache funciona e como configurar as opções fornecidas aos desenvolvedores
ms.localizationpriority: medium
author: sebastienlevert
ms.openlocfilehash: 88b3ed3c8a30f0fcfd79da3cd094420d4534e619
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2022
ms.locfileid: "64589251"
---
# <a name="microsoft-graph-toolkit-caching"></a>Microsoft Graph Toolkit cache

O microsoft Graph Toolkit oferece suporte ao cache de chamadas API do Graph Microsoft. As chamadas estão sendo armazenadas em cache por entidade, como pessoas, contato, foto. Isso permite que um componente recupere os dados e outros componentes para reutilizar sem chamar o Microsoft Graph.

> [!TIP]
> Para obter mais informações sobre quais entidades são armazenadas em cache por cada componente, consulte a documentação do componente.

Bancos de dados criados pelo mgt para cache são prefixados com `mgt-`. Os dados de cada entidade são armazenados em um armazenamento de objetos separado. Para inspecionar o cache, use **a** guia Aplicativo no painel do desenvolvedor (ferramentas F12) - na seção Armazenamento, clique na **guia IndexedDB**. 

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a>Configuração de cache

Você pode ler e gravar as opções de cache por meio do objeto de classe estática `CacheService.config` . Ele é formatado conforme mostrado.

```TypeScript
let config = {
  defaultInvalidationPeriod: number,
  isEnabled: boolean,
  people: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  photos: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  users: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  presence: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  groups: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  response: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  files: {
    invalidationPeriod: number,
    isEnabled: boolean
  },
  fileLists: {
    invalidationPeriod: number,
    isEnabled: boolean
  }
};
```

Períodos de invalidação de cache individuais `null` são padrão no objeto config e padrão para o valor geral `defaultInvalidationPeriod` de 3.600.000 ms (60 minutos). Qualquer valor passado para substituirá `config.x.invalidationPeriod` `defaultInvalidationPeriod`.

O armazenamento de presença é a única exceção e tem um valor padrão de 300000 ms ou 5 minutos.

### <a name="examples"></a>Exemplos

Para desabilitar individualmente um armazenamento, basta definir o `isEnabled` valor das propriedades de config desse armazenamento como false:
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
Desabilitar o cache **não limpa** o cache.

Alterar o período de invalidação é semelhante:

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a>Limpar o cache

O cache é automaticamente limpo quando o usuário sai. Ele também pode ser limpo manualmente.

Se limpar todos os armazenamentos no cache, `clearCaches()` `CacheService` o método da classe limpará todos os armazenamentos mantidos pelo CacheService.

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a>Criando seus próprios armazenamentos de cache

Se você quiser criar e preencher seus próprios armazenamentos de cache para seus componentes personalizados, você pode usar a classe `CacheService` estática.

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> **Observação:** A `storeName` referência que você faz na chamada deve `getCache()` corresponder a um dos armazenamentos listados em seu `CacheSchema` objeto.

O `CacheSchema` objeto é um dicionário com os pares de chave/valor.

```TypeScript
import { CacheSchema } from '@microsoft/mgt';
const cacheSchema: CacheSchema = {
  name: string,
  stores: {
    store1: {},
    store2: {},
    ...
  },
  version: number
};
```

O exemplo a seguir mostra a implementação do cache.

```TypeScript
import { CacheItem, CacheSchema, CacheService, CacheStore } from '@microsoft/mgt';

const cacheSchema: CacheSchema = {
  name: 'users',
  stores: {
    users: {},
    usersQuery: {}
  },
  version: 1
};

interface CacheUser extends CacheItem {
  user?: string;
}

// retrieves invalidation time from cache config
const getUserInvalidationTime = (): number =>
  CacheService.config.users.invalidationPeriod || CacheService.config.defaultInvalidationPeriod;

// checks for if cache is enabled
const usersCacheEnabled = (): boolean => CacheService.config.users.isEnabled && CacheService.config.isEnabled;

// declare the desired cache store
let cache: CacheStore<CacheUser>

// check if the cache is enabled
if (usersCacheEnabled()) {
  cache = CacheService.getCache<CacheUser>(cacheSchema, 'users');
  const user = await cache.getValue(query);

  // check if an item is retrieved, and if it's not expired
  if (user && getUserInvalidationTime() > Date.now() - user.timeCached) {
    return JSON.parse(user.user);
  }
}

// graph call
const graphRes = graph
  .api('me')
  .middlewareOptions(prepScopes('user.read'))
  .get();

// store graph result into the cache if cache is enabled
if (usersCacheEnabled()) {
  cache.putValue(userId, { user: JSON.stringify(graphRes) });
}
```
