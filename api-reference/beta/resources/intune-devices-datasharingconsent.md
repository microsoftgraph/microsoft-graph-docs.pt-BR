---
title: tipo de recurso de dataSharingConsent
description: Informações de consentimento do compartilhamento de dados.
author: tfitzmac
ms.openlocfilehash: 250ad388a5c619a6fd2753d172734145ea720776
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342930"
---
# <a name="datasharingconsent-resource-type"></a>tipo de recurso de dataSharingConsent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





