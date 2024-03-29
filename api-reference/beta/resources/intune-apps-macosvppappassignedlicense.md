---
title: Tipo de recurso macOsVppAppAssignedLicense
description: Atribuição de licença do Programa de Compra de Volume do MacOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d1634285f7364fa063f39ea0272ecf8fc087c52
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59064480"
---
# <a name="macosvppappassignedlicense-resource-type"></a>Tipo de recurso macOsVppAppAssignedLicense

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atribuição de licença do Programa de Compra de Volume do MacOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar macOsVppAppAssignedLicenses](../api/intune-apps-macosvppappassignedlicense-list.md)|[Coleção macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Listar propriedades e relações dos [objetos macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|
|[Obter macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-get.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Ler propriedades e relações do [objeto macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|
|[Criar macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-create.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Crie um novo [objeto macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|
|[Excluir macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-delete.md)|Nenhum|Exclui um [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).|
|[Atualizar macOsVppAppAssignedLicense](../api/intune-apps-macosvppappassignedlicense-update.md)|[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)|Atualize as propriedades de [um objeto macOsVppAppAssignedLicense.](../resources/intune-apps-macosvppappassignedlicense.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
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
  "@odata.type": "microsoft.graph.macOsVppAppAssignedLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```



