---
title: 'Paginação de dados do Microsoft Graph em seu aplicativo '
description: 'Propriedade odata.nextLink` na resposta que contém uma URL para a próxima página de resultados. '
author: FaithOmbongi
ms.localizationpriority: high
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 82d891298a3c33b0bb496c5ad8a1475ecd295934
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65208859"
---
# <a name="paging-microsoft-graph-data-in-your-app"></a>Paginação de dados do Microsoft Graph em seu aplicativo 

Algumas consultas no Microsoft Graph retornam várias páginas de dados devido à paginação do lado do servidor ou devido ao uso do parâmetro de consulta `$top` para limitar especificamente o tamanho da página em uma solicitação. Quando mais de uma solicitação de consulta é necessária para recuperar todos os resultados, o Microsoft Graph retorna uma propriedade `@odata.nextLink` na resposta que contém uma URL para a próxima página de resultados. 

Por exemplo, a URL a seguir solicita todos os usuários em uma organização com o tamanho de página 5 especificado com o parâmetro de consulta `$top`:

```html
https://graph.microsoft.com/v1.0/users?$top=5
```

Se o resultado contiver mais resultados, o Microsoft Graph retornará uma propriedade `@odata.nextLink` semelhante à seguinte junto com a primeira página de resultados:

```json
"@odata.nextLink": "https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27"
```

Você pode recuperar a próxima página de resultados enviando o valor de URL da propriedade `@odata.nextLink` para o Microsoft Graph. 

```html
https://graph.microsoft.com/v1.0/users?$top=5&$skiptoken=X%274453707 ... 6633B900000000000000000000%27
```

O Microsoft Graph continuará a retornar uma referência à próxima página de resultados na propriedade `@odata.nextLink` com cada resposta até que todas as páginas dos resultados tenham sido lidas. Para ler todos os resultados, você deve continuar para todo o Microsoft Graph com a propriedade `@odata.nextLink` retornada em cada resposta até que a propriedade `@odata.nextLink` não seja mais retornada.

>**Importante:** Você deve incluir a URL inteira na propriedade `@odata.nextLink` na solicitação da próxima página de resultados. Dependendo da API em relação à qual a consulta está sendo realizada, o valor de URL `@odata.nextLink` conterá um parâmetro de consulta `$skiptoken` ou `$skip`. A URL também contém todos os outros parâmetros de consulta presentes na solicitação original. Não tente extrair o valor `$skiptoken` ou `$skip` e usá-lo em uma solicitação diferente. 

O comportamento de paginação varia entre diferentes APIs do Microsoft Graph. Ao trabalhar com dados paginados, considere o seguinte:

- Uma página de resultados pode conter zero ou mais resultados.
- APIs diferentes podem ter tamanhos padrão e máximo de página diferentes.
- APIs diferentes poderão se comportar de maneira diferente se você especificar um tamanho de página (por meio do parâmetro de consulta `$top`) que exceda o tamanho máximo de página para essa API. Dependendo da API, o tamanho de página solicitado pode ser ignorado, ele pode usar por padrão o tamanho máximo de página para essa API ou o Microsoft Graph pode retornar um erro. 
- Nem todos os recursos ou relações dão suporte à paginação. Por exemplo, consultas em relação a [directoryRoles](/graph/api/resources/directoryrole) não dão suporte à paginação. Isso inclui os objetos de função de leitura e os membros de função.
- Ao fazer paginação em recursos de diretório, quaisquer cabeçalhos de solicitação adicionais, como o cabeçalho **ConsistencyLevel**, não são incluídos por padrão em solicitações de página subsequentes. Se esses cabeçalhos precisam ser enviados em solicitações subsequentes, você deve defini-los explicitamente.
- Ao usar a cadeia de consulta `$count=true` ao consultar recursos de diretório, a propriedade `@odata.count` estará presente apenas na primeira página dos dados paginados.

## <a name="learn-more-about-paging"></a>Saiba mais sobre paginação
O vídeo a seguir apresenta a paginação no Microsoft Graph.

> [!VIDEO https://www.youtube-nocookie.com/embed/DB_NoC9a1JI]
