---
title: tipo de recurso de contrato
description: Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: b58bd212dd4960bdb5e19967f3b43237caf384ce
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451435"
---
# <a name="agreement-resource-type"></a>tipo de recurso de contrato

Namespace: microsoft.graph

Representa os termos de uso personalizáveis de um locatário que são criados e gerenciados com Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso Azure Active Directory [termos de uso](/azure/active-directory/conditional-access/terms-of-use) de acordo com seu cenário.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar](../api/termsofusecontainer-list-agreements.md) | [coleção agreement](agreement.md) | Obter uma coleção de objetos de contrato. |
| [Criar](../api/termsofusecontainer-post-agreements.md) | [agreement](agreement.md) | Crie um novo contrato postando na coleção de contratos. |
| [Get](../api/agreement-get.md) | [agreement](agreement.md) | Ler propriedades e relações de um objeto de contrato. |
| [Atualizar](../api/agreement-update.md) | Nenhum(a) | Atualize um objeto agreement. |
| [Delete](../api/agreement-delete.md) | Nenhum | Excluir um objeto agreement. |
|[Aceitação de lista](../api/agreement-list-acceptances.md)|Coleção [agreementAcceptance](../resources/agreementacceptance.md)|Obter os detalhes sobre os registros de aceitação de um contrato específico.|
|[Listar agreementAcceptances](../api/user-list-agreementacceptances.md)|Coleção [agreementAcceptance](../resources/agreementacceptance.md)|Obter as aceitaçãos de contrato para o usuário in-locar.|
|[Obter agreementFile](../api/agreementfile-get.md)|[Coleção agreementFile](../resources/agreementfile.md)|Recupere os detalhes do arquivo padrão para um contrato, incluindo as informações de idioma e versão.|
|[Listar arquivos](../api/agreement-list-files.md)|[Coleção agreementFileLocalization](../resources/agreementfilelocalization.md)|Recupere todos os arquivos localizados relacionados a um contrato.|
|[Criar agreementFileLocalization](../api/agreement-post-files.md)|[agreementFileLocalization](../resources/agreementfilelocalization.md)|Crie um novo arquivo de contrato localizado.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|Nome de exibição do contrato. O nome de exibição é usado para o controle interno do contrato, mas não é mostrado aos usuários finais que visualizam o contrato. Suporta `$filter` (`eq`).|
|id|Cadeia de caracteres| O identificador do contrato. Somente leitura. Suporta `$filter` (`eq`).|
|isPerDeviceAcceptanceRequired|Booliano|Indica se os usuários finais são necessários para aceitar esse contrato em todos os dispositivos de onde eles o acessam. O usuário final deve registrar seu dispositivo no Azure AD, caso ainda não tenha feito isso. Suporta `$filter` (`eq`).|
|isViewingBeforeAcceptanceRequired|Booliano|Indica se o usuário precisa expandir o contrato antes de aceitar. Suporta `$filter` (`eq`).|
|termsExpiration|[termsExpiration](termsexpiration.md)| Cronograma de expiração e frequência de acordo para todos os usuários. Suporta `$filter` (`eq`).|
|userReacceptRequiredFrequency|Duration|A duração após a qual o usuário deve aceitar os termos de uso. O valor é representado no formato ISO 8601 por durações. Suporta `$filter` (`eq`).|


## <a name="relationships"></a>Relações
| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|acceptances|Coleção [agreementAcceptance](agreementacceptance.md)|Somente leitura. Informações sobre as aceitaçãos deste contrato.|
|file|[agreementFile](agreementfile.md) | PDF padrão vinculado a este contrato.|
|arquivos|[Coleção agreementFileLocalization](agreementfilelocalization.md)| PDFs vinculados a este contrato. Essa propriedade está em processo de preterido. Use a  **propriedade file** em vez disso. Suporta o `$expand`.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agreement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agreement",
  "id": "String (identifier)",
  "displayName": "String",
  "termsExpiration": {
    "@odata.type": "microsoft.graph.termsExpiration"
  },
  "userReacceptRequiredFrequency": "String (duration)",
  "isViewingBeforeAcceptanceRequired": "Boolean",
  "isPerDeviceAcceptanceRequired": "Boolean"
}
```
