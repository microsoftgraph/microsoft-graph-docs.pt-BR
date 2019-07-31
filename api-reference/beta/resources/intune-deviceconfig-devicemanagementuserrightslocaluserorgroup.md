---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e41a5dbf5d4756e7c635bfdf87aca46f54d8139f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35970406"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="8296d-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="8296d-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="8296d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8296d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8296d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8296d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8296d-106">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="8296d-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="8296d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8296d-107">Properties</span></span>
|<span data-ttu-id="8296d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8296d-108">Property</span></span>|<span data-ttu-id="8296d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8296d-109">Type</span></span>|<span data-ttu-id="8296d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8296d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8296d-111">name</span><span class="sxs-lookup"><span data-stu-id="8296d-111">name</span></span>|<span data-ttu-id="8296d-112">String</span><span class="sxs-lookup"><span data-stu-id="8296d-112">String</span></span>|<span data-ttu-id="8296d-113">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="8296d-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="8296d-114">descrição</span><span class="sxs-lookup"><span data-stu-id="8296d-114">description</span></span>|<span data-ttu-id="8296d-115">String</span><span class="sxs-lookup"><span data-stu-id="8296d-115">String</span></span>|<span data-ttu-id="8296d-116">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="8296d-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="8296d-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="8296d-117">securityIdentifier</span></span>|<span data-ttu-id="8296d-118">String</span><span class="sxs-lookup"><span data-stu-id="8296d-118">String</span></span>|<span data-ttu-id="8296d-119">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="8296d-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8296d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="8296d-120">Relationships</span></span>
<span data-ttu-id="8296d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8296d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8296d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8296d-122">JSON Representation</span></span>
<span data-ttu-id="8296d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8296d-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





