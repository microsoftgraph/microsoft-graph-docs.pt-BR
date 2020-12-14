---
title: Cache do Microsoft Graph Toolkit
description: Explicar como o cache funciona e como configurar as opções fornecidas aos desenvolvedores
localization_priority: Normal
author: adchau
ms.openlocfilehash: f51b4f188fe8ec70f75a50e1d9de049459c97e14
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658702"
---
# <a name="microsoft-graph-toolkit-caching"></a><span data-ttu-id="93b53-103">Cache do Microsoft Graph Toolkit</span><span class="sxs-lookup"><span data-stu-id="93b53-103">Microsoft Graph Toolkit caching</span></span>

<span data-ttu-id="93b53-104">O Microsoft Graph Toolkit oferece suporte a cache de chamadas de API SELECT do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="93b53-104">The Microsoft Graph Toolkit supports caching of select Microsoft Graph API calls.</span></span> <span data-ttu-id="93b53-105">Atualmente, as chamadas para os pontos de extremidade de usuários, pessoas, contatos e fotos são armazenadas em cache por padrão em três repositórios do IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="93b53-105">Currently, calls to the users, person, contact, and photo endpoints are cached by default in three IndexedDB stores.</span></span>

<span data-ttu-id="93b53-106">Você pode exibir o cache no painel de desenvolvedor.</span><span class="sxs-lookup"><span data-stu-id="93b53-106">You can view the cache on the developer panel.</span></span> <span data-ttu-id="93b53-107">Na guia **aplicativo** , no painel **armazenamento** , vá para a guia **IndexedDB** .</span><span class="sxs-lookup"><span data-stu-id="93b53-107">On the **Application** tab, in the **Storage** pane, go to the **IndexedDB** tab.</span></span>

![devtools indexedDB](../images/indexedDBpanel.png)

## <a name="cache-configuration"></a><span data-ttu-id="93b53-109">Configuração de cache</span><span class="sxs-lookup"><span data-stu-id="93b53-109">Cache configuration</span></span>

<span data-ttu-id="93b53-110">Você pode ler e gravar as opções de cache por meio do objeto de classe estática `CacheService.config` .</span><span class="sxs-lookup"><span data-stu-id="93b53-110">You can read and write the cache options through the static class `CacheService.config` object.</span></span> <span data-ttu-id="93b53-111">Ele é formatado como mostrado.</span><span class="sxs-lookup"><span data-stu-id="93b53-111">It is formatted as shown.</span></span>

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
};
```

<span data-ttu-id="93b53-112">Os períodos de invalidação de cache individual são padronizados para `null` o objeto config e o padrão é o `defaultInvalidationPeriod` valor geral 3,6 milhões ms (60 minutos).</span><span class="sxs-lookup"><span data-stu-id="93b53-112">Individual cache invalidation periods are defaulted to `null` in the config object, and default to the general `defaultInvalidationPeriod` value of 3,600,000 ms (60 minutes).</span></span> <span data-ttu-id="93b53-113">Qualquer valor passado para `config.x.invalidationPeriod` será substituído `defaultInvalidationPeriod` .</span><span class="sxs-lookup"><span data-stu-id="93b53-113">Any value passed into `config.x.invalidationPeriod` will override `defaultInvalidationPeriod`.</span></span>

<span data-ttu-id="93b53-114">O repositório de presença é a única exceção e tem um valor padrão de 300000 MS ou 5 minutos.</span><span class="sxs-lookup"><span data-stu-id="93b53-114">The presence store is the only exception, and has a default value of 300000 ms, or 5 minutes.</span></span>

### <a name="examples"></a><span data-ttu-id="93b53-115">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93b53-115">Examples</span></span>

<span data-ttu-id="93b53-116">Para desabilitar individualmente um repositório, basta definir o valor das `isEnabled` Propriedades de config da loja como false:</span><span class="sxs-lookup"><span data-stu-id="93b53-116">To individual disable a store simply set the value of `isEnabled` in that store's config properties to false:</span></span>
```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.isEnabled = false;
```
<span data-ttu-id="93b53-117">Desabilitar o cache **não limpa o** cache.</span><span class="sxs-lookup"><span data-stu-id="93b53-117">Disabling the cache does **not** clear the cache.</span></span>

<span data-ttu-id="93b53-118">Alterar o período de invalditation é semelhante:</span><span class="sxs-lookup"><span data-stu-id="93b53-118">Changing the invalditation period is similar:</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.config.users.invalidationPeriod = 1800000;
```

## <a name="clearing-the-cache"></a><span data-ttu-id="93b53-119">Limpando o cache</span><span class="sxs-lookup"><span data-stu-id="93b53-119">Clearing the cache</span></span>

<span data-ttu-id="93b53-120">O cache é automaticamente limpo quando o usuário se desconecta. Ela também pode ser limpa manualmente.</span><span class="sxs-lookup"><span data-stu-id="93b53-120">The cache is automatically cleared when the user signs out. It can also be cleared manually.</span></span>

<span data-ttu-id="93b53-121">Limpar todas as lojas no cache, o `clearCaches()` método da `CacheService` classe limpará todos os repositórios mantidos pelo CacheService.</span><span class="sxs-lookup"><span data-stu-id="93b53-121">The clear all the stores in the cache, the `clearCaches()` method of the `CacheService` class will clear every store maintained by the CacheService.</span></span>

```JavaScript
import { CacheService } from '@microsoft/mgt';

CacheService.clearCaches();
```

## <a name="creating-your-own-cache-stores"></a><span data-ttu-id="93b53-122">Criar seus próprios repositórios de cache</span><span class="sxs-lookup"><span data-stu-id="93b53-122">Creating your own cache stores</span></span>

<span data-ttu-id="93b53-123">Se você deseja criar e preencher seus próprios repositórios de cache para seus componentes personalizados, você pode usar a `CacheService` classe estática.</span><span class="sxs-lookup"><span data-stu-id="93b53-123">If you want to create and populate your own cache stores for your custom components, you can use the `CacheService` static class.</span></span>

```JavaScript
CacheService.getCache(schema: CacheSchema, storeName: String);
```
> <span data-ttu-id="93b53-124">**Observação:** A `storeName` referência que você faz na chamada `getCache()` deve corresponder a uma das lojas listadas em seu `CacheSchema` objeto.</span><span class="sxs-lookup"><span data-stu-id="93b53-124">**Note:** The `storeName` you reference in the call to `getCache()` must match one of the stores listed in your `CacheSchema` object.</span></span>

<span data-ttu-id="93b53-125">O `CacheSchema` objeto é um dicionário com os pares chave/valor.</span><span class="sxs-lookup"><span data-stu-id="93b53-125">The `CacheSchema` object is a dictionary with the key/value pairs.</span></span>

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

<span data-ttu-id="93b53-126">O exemplo a seguir mostra a implementação de cache.</span><span class="sxs-lookup"><span data-stu-id="93b53-126">The following example shows the cache implementation.</span></span>

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
