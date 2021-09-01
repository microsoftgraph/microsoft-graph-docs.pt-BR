---
title: Tipo de recurso iosVppAppAssignedLicense
description: Atribuição de licença do Programa de Compra de Volume do iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a40d788a632ab9d746dba774388e9ab9df4323d9
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820545"
---
# <a name="iosvppappassignedlicense-resource-type"></a>Tipo de recurso iosVppAppAssignedLicense

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de licença do Programa de Compra de Volume do iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppAppAssignedLicenses](../api/intune-apps-iosvppappassignedlicense-list.md)|[Coleção iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Listar propriedades e relações dos [objetos iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|
|[Obter iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-get.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Ler propriedades e relações do objeto [iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|
|[Criar iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-create.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Crie um novo [objeto iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|
|[Excluir iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-delete.md)|Nenhum|Exclui um [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md).|
|[Atualizar iosVppAppAssignedLicense](../api/intune-apps-iosvppappassignedlicense-update.md)|[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|Atualize as propriedades de [um objeto iosVppAppAssignedLicense.](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|userEmailAddress|Cadeia de caracteres|O endereço de email do usuário.|
|userId|Cadeia de caracteres|A ID do usuário.|
|userName|Cadeia de caracteres|O nome do usuário.|
|userPrincipalName|Cadeia de caracteres|O nome da entidade de segurança do usuário.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```



