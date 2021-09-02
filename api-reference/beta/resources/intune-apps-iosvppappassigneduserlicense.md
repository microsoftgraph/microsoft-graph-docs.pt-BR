---
title: Tipo de recurso iosVppAppAssignedUserLicense
description: Atribuição de licença de usuário do Programa de Compra de Volume do iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a933d23410a828609bbb8e14466bd112657afda6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802807"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>Tipo de recurso iosVppAppAssignedUserLicense

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de licença de usuário do Programa de Compra de Volume do iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.


Herda de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|[Coleção iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Listar propriedades e relações dos [objetos iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|
|[Obter iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Ler propriedades e relações do [objeto iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|
|[Criar iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Crie um novo [objeto iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|
|[Excluir iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|Nenhum(a)|Exclui um [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).|
|[Atualizar iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Atualize as propriedades de [um objeto iosVppAppAssignedUserLicense.](../resources/intune-apps-iosvppappassigneduserlicense.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade. Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|Cadeia de caracteres|O endereço de email do usuário. Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|Cadeia de caracteres|A ID do usuário. Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|Cadeia de caracteres|O nome do usuário. Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|Cadeia de caracteres|O nome da entidade de segurança do usuário. Herdado [do iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```



