---
title: Tipo de recurso hardwarePasswordInfo
description: O Intune fornecerá ao cliente a capacidade de configurar configurações de hardware/bios nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7fd663fbcfd721e6fd6ed762d0de2b107503ec2c
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61345346"
---
# <a name="hardwarepasswordinfo-resource-type"></a>Tipo de recurso hardwarePasswordInfo

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O Intune fornecerá ao cliente a capacidade de configurar configurações de hardware/bios nos dispositivos inscritos do Windows 10 Azure Active Directory ingressados.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar hardwarePasswordInfos](../api/intune-deviceconfig-hardwarepasswordinfo-list.md)|[Coleção hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Listar propriedades e relações dos objetos [hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|
|[Obter hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-get.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Leia propriedades e relações do [objeto hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|
|[Criar hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-create.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Crie um novo [objeto hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|
|[Excluir hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-delete.md)|Nenhum|Exclui um [hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md).|
|[Atualizar hardwarePasswordInfo](../api/intune-deviceconfig-hardwarepasswordinfo-update.md)|[hardwarePasswordInfo](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|Atualize as propriedades de um [objeto hardwarePasswordInfo.](../resources/intune-deviceconfig-hardwarepasswordinfo.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo das informações de senha de hardware|
|serialNumber|String|Número de série do dispositivo|
|currentPassword|String|Senha do dispositivo atual|
|previousPasswords|Coleção de cadeias de caracteres|Lista de senhas de dispositivo anterior|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.hardwarePasswordInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwarePasswordInfo",
  "id": "String (identifier)",
  "serialNumber": "String",
  "currentPassword": "String",
  "previousPasswords": [
    "String"
  ]
}
```




