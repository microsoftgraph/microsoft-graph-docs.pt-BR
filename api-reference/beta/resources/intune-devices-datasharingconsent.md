---
title: tipo de recurso dataSharingConsent
description: Informações de consentimento de compartilhamento de dados.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a7dbb15103ac6bfe337bdb370ef91524226ac72d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999993"
---
# <a name="datasharingconsent-resource-type"></a>tipo de recurso dataSharingConsent

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Informações de consentimento de compartilhamento de dados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|coleção [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Listar Propriedades e relações dos objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Obter dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Leia as propriedades e as relações do objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Criar dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Criar um novo objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Excluir dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|Nenhum|Exclui [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[Atualizar dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Atualiza as propriedades de um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Ação consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID de consentimento de compartilhamento de dados|
|objectdisplayname|String|O nome de exibição do fluxo de trabalho do serviço|
|termsUrl|String|O TermsUrl para o consentimento de compartilhamento de dados|
|granted|Booliano|O Estado concedido para o consentimento de compartilhamento de dados|
|grantDateTime|DateTimeOffset|O consentimento de tempo foi concedido para esta conta|
|grantedByUpn|String|O UPN do usuário que concedeu o consentimento para esta conta|
|grantedByUserId|String|O UserId do usuário que concedeu o consentimento para esta conta|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```





