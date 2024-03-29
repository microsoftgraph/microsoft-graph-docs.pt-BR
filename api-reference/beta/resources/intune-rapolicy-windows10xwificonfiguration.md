---
title: Tipo de recurso windows10XWifiConfiguration
description: Windows Perfil de configuração X WifiXml
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e73fc29134616b421c2a344e62d93f6188dc794
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59030155"
---
# <a name="windows10xwificonfiguration-resource-type"></a>Tipo de recurso windows10XWifiConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows Perfil de configuração X WifiXml


Herda de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10XWifiConfigurations](../api/intune-rapolicy-windows10xwificonfiguration-list.md)|[Coleção windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Listar propriedades e relações dos [objetos windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|
|[Obter windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-get.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Leia propriedades e relações do [objeto windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|
|[Criar windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-create.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Crie um novo [objeto windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|
|[Excluir windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-delete.md)|Nenhum|Exclui um [windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md).|
|[Atualizar windows10XWifiConfiguration](../api/intune-rapolicy-windows10xwificonfiguration-update.md)|[windows10XWifiConfiguration](../resources/intune-rapolicy-windows10xwificonfiguration.md)|Atualize as propriedades de um [objeto windows10XWifiConfiguration.](../resources/intune-rapolicy-windows10xwificonfiguration.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|versão|Int32|Versão do perfil Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|displayName|String|Nome de exibição de perfil Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|description|Cadeia de caracteres|Descrição de perfil [Herdada de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|creationDateTime|DateTimeOffset|Perfil DateTime foi criado Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|lastModifiedDateTime|DateTimeOffset|O perfil DateTime foi modificado pela última vez Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|roleScopeTagIds|Conjunto de cadeias de caracteres|Marcas de escopo herdadas [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|
|authenticationCertificateId|Guid|ID do Certificado de Autenticação|
|customXmlFileName|Cadeia de Caracteres|Nome do arquivo Xml personalizado.|
|customXml|Binário|Comandos XML personalizados que configuram a conexão VPN. (Codificação de byte UTF8)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|assignments|[Coleção deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)|A lista de atribuições para o perfil de configuração do dispositivo. Herdado [de deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)|

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



