---
title: tipo de recurso de dataSharingConsent
description: Informações de consentimento do compartilhamento de dados.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf77a252c323ce83c2dcda44ac294161a4fd4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425691"
---
# <a name="datasharingconsent-resource-type"></a>tipo de recurso de dataSharingConsent

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Informações de consentimento do compartilhamento de dados.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|coleção [dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Lista as propriedades e os relacionamentos dos objetos [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Obter dataSharingConsent](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Leia as propriedades e os relacionamentos do objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Criar dataSharingConsent](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Crie um novo objeto de [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[Excluir dataSharingConsent](../api/intune-devices-datasharingconsent-delete.md)|Nenhum|Exclui um [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).|
|[Atualizar dataSharingConsent](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Atualize as propriedades de um objeto [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) .|
|[ação de consentToDataSharing](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O consentimento de compartilhamento de dados Id|
|Nome_para_exibição_do_serviço|String|O nome para exibição do fluxo de trabalho de serviço|
|termsUrl|String|O TermsUrl para os consentimento de compartilhamento de dados|
|concedido|Boolean|O estado foram concedido para os consentimento de compartilhamento de dados|
|grantDateTime|DateTimeOffset|O consentimento de tempo foi concedido para esta conta|
|grantedByUpn|String|O Upn do usuário que tenha concedido consentimento para esta conta|
|grantedByUserId|String|A identificação do usuário do usuário que tenha concedido consentimento para esta conta|

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




