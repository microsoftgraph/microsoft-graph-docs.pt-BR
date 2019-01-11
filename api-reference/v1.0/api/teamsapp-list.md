---
title: Listar os aplicativos publicados a partir do catálogo de aplicativos do Microsoft Teams
description: 'Lista de aplicativos a partir do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 494bc371f88cd15a7c96ff0c145e6593c0716b5c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887057"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a>Listar os aplicativos publicados a partir do catálogo de aplicativos do Microsoft Teams



Listar os [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams. Isso inclui aplicativos do repositório de Teams da Microsoft, bem como aplicativos de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino). Para obter os aplicativos do catálogo de aplicativos da sua organização somente, especifique `Organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).

>**Observação:** Somente os administradores globais podem chamar essa API. 

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)|
|:----------------------------------     |:-------------|
| Delegado (conta corporativa ou de estudante)     | AppCatalog.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte|
| Aplicativo                            | Sem suporte|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a>Parâmetros de consulta opcionais
Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho        | Valor           |
|:--------------|:--------------  |
| Autorização | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Nenhum.

>**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsCatalogApp](../resources/teamsapp.md) para diminuir a lista de resultados. Você pode usar qualquer uma das seguintes operações de filtro: igual, não-igual e, ou e não.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsCatalogApp](../resources/teamsapp.md) no corpo da resposta.

## <a name="examples"></a>Exemplos
### <a name="example-1"></a>Exemplo 1
O exemplo a seguir lista todos os aplicativos que são específicos para seu locatário.

#### <a name="request"></a>Solicitação
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a>Resposta
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a>Exemplo 2

O exemplo a seguir lista aplicativos com uma ID especificada.

#### <a name="request"></a>Solicitação
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a>Resposta
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

