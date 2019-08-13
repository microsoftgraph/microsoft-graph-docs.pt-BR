---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3bf4ac6aa9de235b1e4117b47c6a5eafc5c011a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332747"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="ee3de-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="ee3de-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="ee3de-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ee3de-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ee3de-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ee3de-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee3de-106">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="ee3de-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="ee3de-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee3de-107">Properties</span></span>
|<span data-ttu-id="ee3de-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee3de-108">Property</span></span>|<span data-ttu-id="ee3de-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee3de-109">Type</span></span>|<span data-ttu-id="ee3de-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee3de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee3de-111">name</span><span class="sxs-lookup"><span data-stu-id="ee3de-111">name</span></span>|<span data-ttu-id="ee3de-112">String</span><span class="sxs-lookup"><span data-stu-id="ee3de-112">String</span></span>|<span data-ttu-id="ee3de-113">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="ee3de-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="ee3de-114">descrição</span><span class="sxs-lookup"><span data-stu-id="ee3de-114">description</span></span>|<span data-ttu-id="ee3de-115">String</span><span class="sxs-lookup"><span data-stu-id="ee3de-115">String</span></span>|<span data-ttu-id="ee3de-116">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="ee3de-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="ee3de-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="ee3de-117">securityIdentifier</span></span>|<span data-ttu-id="ee3de-118">String</span><span class="sxs-lookup"><span data-stu-id="ee3de-118">String</span></span>|<span data-ttu-id="ee3de-119">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="ee3de-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee3de-120">Relações</span><span class="sxs-lookup"><span data-stu-id="ee3de-120">Relationships</span></span>
<span data-ttu-id="ee3de-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee3de-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee3de-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee3de-122">JSON Representation</span></span>
<span data-ttu-id="ee3de-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee3de-123">Here is a JSON representation of the resource.</span></span>
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



