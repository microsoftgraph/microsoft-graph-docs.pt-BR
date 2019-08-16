---
title: tipo de recurso roleManagement
description: Recurso de gerenciamento de função RBAC
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bd4e1eefeae819d37630a7faf4fbb1f6d1a5124c
ms.sourcegitcommit: 567d0420243765b4088bc8029306a517f92926fd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/16/2019
ms.locfileid: "36437815"
---
# <a name="rolemanagement-resource-type"></a>tipo de recurso roleManagement

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entidade de gerenciamento de função RBAC da Microsoft 365. Fornece acesso a definições de função e atribuições de função provenientes de provedores de RBAC. Atualmente, só há suporte para o provedor de diretório. Para obter mais informações, consulte [permissões de função de administrador no Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

Nenhuma

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|Directory|[rbacApplication](rbacapplication.md)| Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Nenhuma

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "roleManagement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
