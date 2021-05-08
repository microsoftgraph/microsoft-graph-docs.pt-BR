---
title: O Microsoft Graph Toolkit cache
description: Explicando como o Cache funciona e como configurar as opções fornecidas aos desenvolvedores
localization_priority: Normal
author: adchau
ms.openlocfilehash: cef5c06c39ebad58e6a39f094427dea6a1b1be25
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266617"
---
# <a name="microsoft-graph-toolkit-caching"></a>O Microsoft Graph Toolkit cache

O microsoft graph Toolkit suporta o cache de chamadas de API do Microsoft Graph selecionadas. As chamadas estão sendo armazenadas em cache por entidade, como pessoas, contato, foto. Isso permite que um componente recupere os dados e outros componentes para reutilizar sem chamar o Microsoft Graph.

> [!TIP]
> Para obter mais informações sobre quais entidades são armazenadas em cache por cada componente, consulte a documentação do componente.

Bancos de dados criados pelo mgt para cache são prefixados com `mgt-` . Os dados de cada entidade são armazenados em um armazenamento de objetos separado. Para inspecionar o cache, use a guia Aplicativo no painel do  desenvolvedor (ferramentas F12) - na seção Armazenamento, clique na **guia IndexedDB.**  

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a>Configuração de cache

Você pode ler e gravar as opções de cache por meio do objeto de classe `CacheService.config` estática. Ele é formatado conforme mostrado.

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
  }
};
```

Períodos de invalidação de cache individuais são padrão no objeto config e padrão para o valor geral de `null` `defaultInvalidationPeriod` 3.600.000 ms (60 minutos). Qualquer valor passado para `config.x.invalidationPeriod` substituirá `defaultInvalidationPeriod` .

O armazenamento de presença é a única exceção e tem um valor padrão de 300000 ms ou 5 minutos.

### <a name="examples"></a>Exemplos

Para desabilitar individualmente um armazenamento, basta definir o valor das propriedades de config desse armazenamento `isEnabled` como false:
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
Desabilitar o cache **não limpa** o cache.

Alterar o período de invalditation é semelhante:

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a>Limpar o cache

O cache é automaticamente limpo quando o usuário sai. Ele também pode ser limpo manualmente.

Se limpar todos os armazenamentos no cache, o método da classe limpará todos os `clearCaches()` `CacheService` armazenamentos mantidos pelo CacheService.

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a>Criando seus próprios armazenamentos de cache

Se você quiser criar e preencher seus próprios armazenamentos de cache para seus componentes personalizados, você pode usar a `CacheService` classe estática.

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> **Observação:** A `storeName` referência que você faz na chamada deve corresponder a um dos `getCache()` armazenamentos listados em seu `CacheSchema` objeto.

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
