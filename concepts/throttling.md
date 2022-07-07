---
title: Diretrizes de limitação do Microsoft Graph
description: Encontre práticas recomendadas para manter o desempenho ideal do serviço Microsoft Graph se ocorrer um grande número de solicitações.
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20
ms.openlocfilehash: d26976bad505adfb2564e50609ea5d6186148b4e
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66671364"
---
# <a name="microsoft-graph-throttling-guidance"></a>Diretrizes de limitação do Microsoft Graph

Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.

Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.

> [!NOTE]
> As soluções que precisam extrair um grande volume de dados do Microsoft Graph devem usar o [Microsoft Graph Data Connect](data-connect-concept-overview.md) em vez das APIs REST do Microsoft Graph. O Microsoft Graph Data Connect permite que as organizações extraiam dados do Microsoft 365 em massa sem estarem sujeitas a limites de limitação.

<!-- markdownlint-disable MD033 -->
<br/>

<!-- markdownlint-disable MD034 -->
> [!VIDEO https://www.youtube-nocookie.com/embed/J4CFxVuzNMA]
<!-- markdownlint-enable MD034 -->

<!-- markdownlint-disable MD026 -->
## <a name="what-happens-when-throttling-occurs"></a>O que acontece quando a limitação ocorre?
<!-- markdownlint-enable MD026 -->

Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas.

## <a name="common-throttling-scenarios"></a>Cenários comuns de limitação

As causas mais comuns de limitação dos clientes incluem:

- Um grande número de solicitações em todos os aplicativos em um locatário.
- Um grande número de solicitações de um aplicativo específico entre todos os locatários.

## <a name="sample-response"></a>Resposta de amostra

Sempre que o limite de estrangulamento é excedido, o Microsoft Graph responde com uma resposta semelhante a esta.

```http
HTTP/1.1 429 Too Many Requests
Content-Type: application/json
Retry-After: 10

{
  "error": {
    "code": "TooManyRequests",
    "innerError": {
      "code": "429",
      "date": "2020-08-18T12:51:51",
      "message": "Please retry after",
      "request-id": "94fb3b52-452a-4535-a601-69e0a90e3aa2",
      "status": "429"
    },
    "message": "Please retry again later."
  }
}
```

## <a name="best-practices-to-handle-throttling"></a>Práticas recomendadas para lidar com a limitação

Estas são as práticas recomendadas para lidar com a limitação:

- Reduza o número de operações por solicitação.
- Reduza a frequência de chamadas.
- Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.

Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo `Retry-After` no cabeçalho de resposta. Desativar solicitações usando o atraso `Retry-After` é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.

1. Aguarde o número de segundos especificado no cabeçalho `Retry-After`.
2. Repita a solicitação.
3. Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso `Retry-After` recomendado e repita a solicitação até obter êxito.

Todos os recursos e APIs descritos nos [Limites específicos do serviço](throttling-limits.md) fornecem um cabeçalho `Retry-After`, exceto quando indicado.

Para uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](/azure/architecture/patterns/throttling).

> [!NOTE]
> Se nenhum cabeçalho `Retry-After` for fornecido pela resposta, recomendamos implementar uma política de repetição exponencial de retirada. Você também pode implementar [padrões mais avançados](/azure/architecture/patterns/category/resiliency) ao criar aplicativos em grande escala.
>
> Os SDKs do Microsoft Graph já implementam manipuladores que dependem do cabeçalho `Retry-After` ou padrão para uma política de repetição de retirada exponencial.

## <a name="best-practices-to-avoid-throttling"></a>Práticas recomendadas para evitar a limitação

Padrões de programação, como pesquisar continuamente um recurso para verificar atualizações e verificar regularmente coleções de recursos para verificar recursos novos ou excluídos, são mais propensos a fazer com que os aplicativos sejam limitados e degradem o desempenho geral. Em vez disso, você deve aproveitar [controle de alterações](delta-query-overview.md) e [notificações de alterações](webhooks.md) quando disponíveis.

>[!NOTE]
>[Práticas recomendadas para descobrir arquivos e detectar alterações em escala](/onedrive/developer/rest-api/concepts/scan-guidance) descrevem as práticas recomendadas em detalhes.

## <a name="throttling-and-batching"></a>Limitação e dosagem

[O lote JSON](./json-batching.md) permite que você otimize seu aplicativo combinando várias solicitações em um único objeto JSON. As solicitações em um lote são avaliadas individualmente em relação aos limites de estrangulamento e, se alguma solicitação exceder os limites, ela falhará com um `status` de `429` e um erro semelhante ao fornecido acima. O próprio lote falha com um código de status de `424` (Dependência com Falha). É possível que várias solicitações sejam limitadas em um único lote. Você deve tentar novamente a cada solicitação com falha no lote utilizando o valor fornecido no cabeçalho de resposta `retry-after` do conteúdo JSON. Você pode tentar novamente para todas as solicitações com falha em um novo lote após o valor `retry-after` mais longo.

Se os SDKs tentarem novamente as solicitações limitadas automaticamente quando não estiverem em lote, as solicitações limitadas que fizeram parte de um lote não serão automaticamente repetidas.

## <a name="next-steps"></a>Próximas etapas

Identifique os [limites de limitação](throttling-limits.md) que se aplicam a cada recurso do Microsoft Graph.