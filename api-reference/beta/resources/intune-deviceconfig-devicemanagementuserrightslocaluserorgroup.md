---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: acccbb68ecc0b62d27ac20e3eba9e637aac3e11c
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946935"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="a90c4-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="a90c4-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="a90c4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a90c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a90c4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a90c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a90c4-106">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="a90c4-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="a90c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a90c4-107">Properties</span></span>
|<span data-ttu-id="a90c4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a90c4-108">Property</span></span>|<span data-ttu-id="a90c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a90c4-109">Type</span></span>|<span data-ttu-id="a90c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a90c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a90c4-111">nome</span><span class="sxs-lookup"><span data-stu-id="a90c4-111">name</span></span>|<span data-ttu-id="a90c4-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a90c4-112">String</span></span>|<span data-ttu-id="a90c4-113">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="a90c4-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="a90c4-114">description</span><span class="sxs-lookup"><span data-stu-id="a90c4-114">description</span></span>|<span data-ttu-id="a90c4-115">String</span><span class="sxs-lookup"><span data-stu-id="a90c4-115">String</span></span>|<span data-ttu-id="a90c4-116">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="a90c4-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="a90c4-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="a90c4-117">securityIdentifier</span></span>|<span data-ttu-id="a90c4-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a90c4-118">String</span></span>|<span data-ttu-id="a90c4-119">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="a90c4-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a90c4-120">Relações</span><span class="sxs-lookup"><span data-stu-id="a90c4-120">Relationships</span></span>
<span data-ttu-id="a90c4-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a90c4-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a90c4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a90c4-122">JSON Representation</span></span>
<span data-ttu-id="a90c4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a90c4-123">Here is a JSON representation of the resource.</span></span>
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




