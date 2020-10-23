---
title: tipo de recurso dataSharingConsent
description: Informações de consentimento de compartilhamento de dados.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0235abf74d96e5ccff888253e977bd9951bbc3cd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703647"
---
# <a name="datasharingconsent-resource-type"></a>tipo de recurso dataSharingConsent

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|granted|Boolean|O Estado concedido para o consentimento de compartilhamento de dados|
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





