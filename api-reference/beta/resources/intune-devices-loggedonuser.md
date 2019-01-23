---
title: tipo de recurso de loggedOnUser
description: Usuário conectado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ac0ca08c6d324836e4bb9dd9951fdfe742b8b5f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395192"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="9a7bd-103">tipo de recurso de loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="9a7bd-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="9a7bd-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9a7bd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9a7bd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9a7bd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9a7bd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9a7bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a7bd-107">Usuário conectado</span><span class="sxs-lookup"><span data-stu-id="9a7bd-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="9a7bd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a7bd-108">Properties</span></span>
|<span data-ttu-id="9a7bd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a7bd-109">Property</span></span>|<span data-ttu-id="9a7bd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a7bd-110">Type</span></span>|<span data-ttu-id="9a7bd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a7bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a7bd-112">userId</span><span class="sxs-lookup"><span data-stu-id="9a7bd-112">userId</span></span>|<span data-ttu-id="9a7bd-113">String</span><span class="sxs-lookup"><span data-stu-id="9a7bd-113">String</span></span>|<span data-ttu-id="9a7bd-114">Id de usuário</span><span class="sxs-lookup"><span data-stu-id="9a7bd-114">User id</span></span>|
|<span data-ttu-id="9a7bd-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="9a7bd-115">lastLogOnDateTime</span></span>|<span data-ttu-id="9a7bd-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a7bd-116">DateTimeOffset</span></span>|<span data-ttu-id="9a7bd-117">Data e hora de quando o usuário fizer logon</span><span class="sxs-lookup"><span data-stu-id="9a7bd-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a7bd-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9a7bd-118">Relationships</span></span>
<span data-ttu-id="9a7bd-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a7bd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a7bd-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a7bd-120">JSON Representation</span></span>
<span data-ttu-id="9a7bd-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a7bd-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




