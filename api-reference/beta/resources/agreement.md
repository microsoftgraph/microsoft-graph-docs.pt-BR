---
title: tipo de recurso de contrato
description: Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: c3d4fae159ef6c4187d042b97c02d8332b0af0d9
ms.sourcegitcommit: 9759b647acfbed99d5675a6f512aaa33932a723f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/23/2021
ms.locfileid: "61604319"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso Azure Active Directory [termos de uso](/azure/active-directory/conditional-access/terms-of-use) de acordo com seu cenário.

## <a name="methods"></a>Methods

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Criar acordos](../api/agreement-post-agreements.md) | [agreement](agreement.md) | Crie um novo contrato postando na coleção de contratos. |
| [Listar contratos](../api/agreement-list.md) | [coleção agreement](agreement.md) | Obter uma coleção de objetos de contrato. |
| [Obter contrato](../api/agreement-get.md) | [agreement](agreement.md) | Ler propriedades e relações de um objeto de contrato. |
| [Atualizar contrato](../api/agreement-update.md) | [agreement](agreement.md) | Atualize um objeto agreement. |
| [Excluir contrato](../api/agreement-delete.md) | Nenhum | Excluir um objeto agreement. |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome de exibição do contrato. O nome de exibição é usado para o controle interno do contrato, mas não é mostrado aos usuários finais que visualizam o contrato.|
|id|String| Somente leitura.|
|isPerDeviceAcceptanceRequired|Booliano|Essa configuração permite exigir que os usuários finais aceitem esse contrato em todos os dispositivos de onde eles estão acessando. O usuário final será necessário para registrar seu dispositivo no Azure AD, caso ainda não tenha feito isso.|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário precisa expandir o contrato antes de aceitar.|
|termsExpiration|[termsExpiration](termsexpiration.md)| Cronograma de expiração e frequência de acordo para todos os usuários. |
|userReacceptRequiredFrequency|Duração|A duração após a qual o usuário deve aceitar os termos de uso. O valor é representado no formato ISO 8601 por durações.|


## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|acceptances|Coleção [agreementAcceptance](agreementacceptance.md)|Somente leitura. Informações sobre as aceitaçãos deste contrato.|
|arquivos|[Coleção agreementFileLocalization](agreementfilelocalization.md)| PDFs vinculados a este contrato. **Observação:** Essa propriedade está em processo de preterido. Use a  **propriedade file** em vez disso.|
|file|[agreementFile](agreementfile.md) | PDF padrão vinculado a este contrato.|
|file/localizações|[Coleção agreementFileLocalization](agreementfilelocalization.md)|As versões localizadas dos arquivos de contrato anexados ao contrato.|
|file/localizations/{localizationId}/versions|[Coleção agreementFileVersion](agreementfileversion.md)|O histórico de versão do arquivo de contrato localizado.|


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


