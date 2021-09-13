---
title: Tipo de recurso deviceManagementDomainJoinConnector
description: Um Conector de Junção de Domínio é um conector responsável por alocar (e excluir) blobs de conta de máquina
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d638537c50c10a9e8a520cd9dc50316e7e3e3f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59017272"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a>Tipo de recurso deviceManagementDomainJoinConnector

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um Conector de Junção de Domínio é um conector responsável por alocar (e excluir) blobs de conta de máquina

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementDomainJoinConnectors](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|[Coleção deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Listar propriedades e relações dos [objetos deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|
|[Obter deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Leia propriedades e relações do [objeto deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|
|[Criar deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Crie um novo [objeto deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|
|[Excluir deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|None|Exclui um [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).|
|[Atualizar deviceManagementDomainJoinConnector](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|Atualize as propriedades de [um objeto deviceManagementDomainJoinConnector.](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para representar um conector.|
|displayName|Cadeia de caracteres|O nome de exibição do conector.|
|lastConnectionDateTime|DateTimeOffset|Última vez que o conector entrou em contato com o Intune.|
|state|[deviceManagementDomainJoinConnectorState](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|O estado do conector. Os valores possíveis são: `active`, `error`, `inactive`.|
|versão|String|A versão do conector.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```



