---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: af4a6079aaed846af3322a94eb961315f7291686
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617098"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](/azure/active-directory/active-directory-tou) acordo com seu cenário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar contratos](../api/agreement-post-agreements.md) | [contrato](agreement.md) | Crie um novo contrato postando na coleção de contratos. |
| [Listar contratos](../api/agreement-list.md) | coleção de [contratos](agreement.md) | Obtenha uma coleção de objetos de contrato. |
| [Obter contrato](../api/agreement-get.md) | [contrato](agreement.md) | Leia as propriedades e as relações de um objeto de contrato. |
| [Atualizar contrato](../api/agreement-update.md) | [contrato](agreement.md) | Atualize um objeto de contrato. |
| [Excluir contrato](../api/agreement-delete.md) | Nenhum | Exclua um objeto de contrato. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome para exibição do contrato. O nome para exibição é usado para o controle interno do contrato, mas não é exibido para os usuários finais que exibem o contrato.|
|id|String| Somente leitura.|
|isPerDeviceAcceptanceRequired|Booliano|Essa configuração permite que você exija que os usuários finais aceitem este contrato em todos os dispositivos dos quais eles estão acessando-os. O usuário final será solicitado a registrar o dispositivo no Azure AD, caso ainda não tenha feito isso.|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário tem que expandir o contrato antes de aceitar.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Cronograma de expiração e frequência de contrato para todos os usuários. |
|userReacceptRequiredFrequency|Duração|A duração após a qual o usuário deve aceitar novamente os termos de uso. O valor é representado no formato ISO 8601 para durações.|


## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|aceitação|Coleção [agreementAcceptance](agreementacceptance.md)|Somente leitura. Informações sobre as aceitações deste contrato.|
|arquivos|coleção [agreementFileLocalization](agreementfilelocalization.md)| PDFs vinculados a este contrato. **Observação:** Essa propriedade está no processo de ser preterido. Em vez disso, use a propriedade  **File** .|
|file|[agreementFile](agreementfile.md) | PDF padrão vinculado a este contrato.|
|arquivos/localizações|coleção [agreementFileLocalization](agreementfilelocalization.md)|As versões localizadas dos arquivos de contrato anexados ao contrato.|
|arquivo/localizações/{localizações}/versões|coleção [agreementFileVersion](agreementfileversion.md)|O histórico de versão do arquivo de contrato localizado.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


