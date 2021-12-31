---
title: Tipo de recurso accessPackageSubject
description: No gerenciamento de direitos do Azure AD, um assunto de uma atribuição de pacote de acesso.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 5092494b1c5f496a1ee3abf76800dbb8a05f49ff
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651179"
---
# <a name="accesspackagesubject-resource-type"></a>Tipo de recurso accessPackageSubject

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-overview.md)um assunto do pacote de acesso é um usuário, entidade de serviço ou outra entidade que pode ser configurada para solicitar ou ter um pacote de acesso atribuído.  Ele pode representar um solicitante de uma organização conectada que ainda não está no locatário.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|String|O nome de exibição do assunto.|
|email|Cadeia de caracteres|O endereço de email do assunto.|
|id|String| Somente leitura.|
|objectId|Cadeia de caracteres|O identificador de objeto do assunto. `null` se o assunto ainda não for um usuário no locatário.|
|principalName|Cadeia de caracteres|O nome principal, se conhecido, do assunto.|
|type|String|O tipo de recurso do assunto.|
|connectedOrganizationId|String|O identificador da organização conectada do assunto.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|connectedOrganization|[connectedOrganization](connectedorganization.md)| A organização conectada do assunto. Somente leitura. Anulável.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "Administrator",
  "email": "admin@contoso.com",
  "id": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
  "objectId": "cc754ed5-f598-45c0-aaf0-fc2f2eb1838f",
  "principalName": "admin@domain.contoso.com",
  "type": "User"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageSubject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

