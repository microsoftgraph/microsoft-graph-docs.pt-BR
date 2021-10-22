---
title: Tipo de recurso remoteAssistancePartner
description: Os recursos RemoteAssistPartner representam os metadados e o status de um determinado serviço de parceiro de Assistência Remota.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6857d47fbed69bc74d92bce1e7ccb63dc84059e1
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60448938"
---
# <a name="remoteassistancepartner-resource-type"></a>Tipo de recurso remoteAssistancePartner

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Os recursos RemoteAssistPartner representam os metadados e o status de um determinado serviço de parceiro de Assistência Remota.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar remoteAssistancePartners](../api/intune-remoteassistance-remoteassistancepartner-list.md)|Conjunto [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Obter remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Ler propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Criar remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Criar um novo objeto de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Excluir remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|Nenhum|Excluir [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Atualizar remoteAssistancePartner](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md)|Atualizar as propriedades de um objeto de [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).|
|[Ação beginOnboarding](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|Nenhum|Uma solicitação para iniciar a integração.  Deve estar juntamente com as informações apropriadas da conta do TeamViewer|
|[ação de desconectar](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|Nenhum|Uma solicitação para remover o conector ativo do TeamViewer|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do parceiro.|
|displayName|Cadeia de caracteres|Nome de exibição do parceiro.|
|onboardingUrl|Cadeia de caracteres|URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|Uma descrição amigável do status atual do conector teamViewer. Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```



