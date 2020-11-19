---
title: tipo de recurso windows10XWifiConfiguration
description: Perfil de configuração do Windows X WifiXml
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1353597c05d1f661474f563b6dee3c07fe408f77
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301409"
---
# <a name="windows10xwificonfiguration-resource-type"></a>tipo de recurso windows10XWifiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração do Windows X WifiXml


Herda de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10XWifiConfigurations](../api/intune-rapolicy-windows10xwificonfiguration-list.md)|coleção [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Listar Propriedades e relações dos objetos [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|
|[Obter windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-get.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Leia as propriedades e as relações do objeto [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|
|[Criar windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-create.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Criar um novo objeto [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|
|[Excluir windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-delete.md)|Nenhum|Exclui [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md).|
|[Atualizar windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-update.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Atualiza as propriedades de um objeto [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|versão|Int32|Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|String|Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDatetime|DateTimeOffset|O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Coleção de cadeias de caracteres|Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|authenticationCertificateId|Guid|ID para o certificado de autenticação|
|customXmlFileName|String|Nome de arquivo XML personalizado.|
|customXml|Binária|Comandos XML personalizados que configura a conexão VPN. (Codificação de bytes UTF8)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|coleção [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XWifiConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XWifiConfiguration",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "authenticationCertificateId": "Guid",
  "customXmlFileName": "String",
  "customXml": "binary"
}
```




