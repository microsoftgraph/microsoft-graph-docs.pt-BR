---
title: Tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: d9c19bc431ce152bb3b15f97822ee86071c314d8
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2022
ms.locfileid: "65061115"
---
# <a name="synchronizationjobsubject-resource-type"></a>Tipo de recurso synchronizationJobSubject

Namespace: microsoft.graph

Representa os objetos que serão provisionados durante o provisionamento sob demanda.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|objectId|Cadeia de caracteres|O identificador de um objeto ao qual um **synchronizationJob** deve ser aplicado. Pode ser um dos seguintes: <li>Um **onPremisesDistinguishedName** para sincronização do Active Directory para o Azure AD.</li><li>A ID de usuário para sincronização do Azure AD para terceiros.</li><li>A ID de trabalho do trabalho do Workday para sincronização do Workday para o Active Directory ou o Azure AD.</li>|
|objectTypeName|Cadeia de caracteres|O tipo do objeto ao qual um **synchronizationJob** deve ser aplicado. Pode ser um dos seguintes: <li>`user` para sincronização do Active Directory para o Azure AD.</li><li>`User` para sincronização do Azure AD para um aplicativo de terceiros. </li><li>`Worker` para sincronização do Workday para o Active Directory ou o Azure AD.</li>|

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
  "objectTypeName": "String"
}
```


