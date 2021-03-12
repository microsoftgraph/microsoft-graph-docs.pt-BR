---
title: tipo de recurso de contrato
description: Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 045d4b9142d4bd0c4bc01392975871e0253d33c0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722556"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

Namespace: microsoft.graph

Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com o Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso Termos de Uso do [Azure Active Directory](/azure/active-directory/active-directory-tou) de acordo com seu cenário.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar contratos](../api/agreement-list.md) | [coleção agreement](agreement.md) | Obter uma coleção de objetos de contrato. |
| [Criar acordos](../api/agreement-post-agreements.md) | [agreement](agreement.md) | Crie um novo contrato postando na coleção de contratos. |
| [Obter contrato](../api/agreement-get.md) | [agreement](agreement.md) | Ler propriedades e relações de um objeto de contrato. |
| [Atualizar contrato](../api/agreement-update.md) | [agreement](agreement.md) | Atualize um objeto agreement. |
| [Excluir contrato](../api/agreement-delete.md) | Nenhum | Excluir um objeto agreement. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome de exibição do contrato. O nome de exibição é usado para o controle interno do contrato, mas não é mostrado aos usuários finais que visualizam o contrato.|
|id|Cadeia de caracteres| O identificador do contrato. Somente leitura.|
|isPerDeviceAcceptanceRequired|Booliano|Indica se os usuários finais são necessários para aceitar esse contrato em todos os dispositivos de onde eles o acessam. O usuário final deve registrar seu dispositivo no Azure AD, caso ainda não tenha feito isso.|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário precisa expandir o contrato antes de aceitar.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Cronograma de expiração e frequência de acordo para todos os usuários. |
|userReacceptRequiredFrequency|Duration|A duração após a qual o usuário deve aceitar os termos de uso. O valor é representado no formato ISO 8601 por durações.|


## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|acceptances|Coleção [agreementAcceptance](agreementacceptance.md)|Somente leitura. Informações sobre as aceitaçãos deste contrato.|
|arquivos|[Coleção agreementFileLocalization](agreementfilelocalization.md)| PDFs vinculados a este contrato. Essa propriedade está em processo de preterido. Use a  **propriedade file** em vez disso.|
|file|[agreementFile](agreementfile.md) | PDF padrão vinculado a este contrato.|
|localizações|[Coleção agreementFileLocalization](agreementfilelocalization.md)|As versões localizadas dos arquivos de contrato anexados ao contrato.|
|versões|[Coleção agreementFileVersion](agreementfileversion.md)|O histórico de versão do arquivo de contrato localizado.|


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


