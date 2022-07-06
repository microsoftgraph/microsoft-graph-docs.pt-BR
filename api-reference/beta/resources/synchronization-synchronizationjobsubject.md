---
title: Tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 33316bfb434d34c8f367832f9334938cf1c0cf8b
ms.sourcegitcommit: cf2b3c67cb9ce832944cfbac66171590bbbd83de
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/06/2022
ms.locfileid: "66645419"
---
# <a name="synchronizationjobsubject-resource-type"></a>Tipo de recurso synchronizationJobSubject

Namespace: microsoft.graph

Representa os objetos que serão provisionados durante o provisionamento sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|links|[synchronizationLinkedObjects](../resources/synchronization-synchronizationlinkedobjects.md)|Entidades de segurança que você gostaria de provisionar.|
|objectId|Cadeia de caracteres|O identificador de um objeto ao qual um **synchronizationJob** deve ser aplicado. Pode ser um dos seguintes: <li>Um **onPremisesDistinguishedName** para sincronização do Active Directory para o Azure AD.</li><li>A ID de usuário para sincronização Azure AD para terceiros.</li><li>A ID de trabalho do trabalho do Workday para sincronização do Workday para o Active Directory ou Azure AD.</li>|
|objectTypeName|Cadeia de caracteres|O tipo do objeto ao qual um **synchronizationJob** deve ser aplicado. Pode ser um dos seguintes: <li>`user`para sincronizar entre o Active Directory e o Azure AD.</li><li>`User`para sincronizar um usuário entre Azure AD e um aplicativo de terceiros. </li><li>`Worker`para sincronização de um usuário entre o Workday e o Active Directory ou Azure AD.</li><li>`Group`para sincronizar um grupo entre Azure AD e um aplicativo de terceiros. </li>|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String",
  "links": {
    "@odata.type": "microsoft.graph.synchronizationLinkedObjects"
  }
}
```


