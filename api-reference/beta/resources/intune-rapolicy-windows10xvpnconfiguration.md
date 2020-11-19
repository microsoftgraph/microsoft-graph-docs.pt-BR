---
title: tipo de recurso windows10XVpnConfiguration
description: Perfil de configuração da VPN do Windows X
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cce0be552b22e52476ee704606bd43e7c20f4ec7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301607"
---
# <a name="windows10xvpnconfiguration-resource-type"></a>tipo de recurso windows10XVpnConfiguration

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Perfil de configuração da VPN do Windows X


Herda de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10XVpnConfigurations](../api/intune-rapolicy-windows10xvpnconfiguration-list.md)|coleção [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Listar Propriedades e relações dos objetos [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|
|[Obter windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-get.md)|[windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Leia as propriedades e as relações do objeto [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|
|[Criar windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-create.md)|[windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Criar um novo objeto [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|
|[Excluir windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-delete.md)|Nenhum|Exclui [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md).|
|[Atualizar windows10XVpnConfiguration](../api/intune-rapolicy-windows10xvpnconfiguration-update.md)|[windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md)|Atualiza as propriedades de um objeto [windows10XVpnConfiguration](../resources/intune-rapolicy-windows10xvpnconfiguration.md) .|

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
  "@odata.type": "microsoft.graph.windows10XVpnConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XVpnConfiguration",
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




