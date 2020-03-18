---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 49721c0713bcb2b2af7b3b19fbcb3c2f4a816194
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42792000"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="4ec05-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="4ec05-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="4ec05-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4ec05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ec05-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4ec05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ec05-106">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ec05-106">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="4ec05-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ec05-107">Properties</span></span>
|<span data-ttu-id="4ec05-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ec05-108">Property</span></span>|<span data-ttu-id="4ec05-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ec05-109">Type</span></span>|<span data-ttu-id="4ec05-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ec05-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ec05-111">nome</span><span class="sxs-lookup"><span data-stu-id="4ec05-111">name</span></span>|<span data-ttu-id="4ec05-112">String</span><span class="sxs-lookup"><span data-stu-id="4ec05-112">String</span></span>|<span data-ttu-id="4ec05-113">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="4ec05-113">The name of this local user or group.</span></span>|
|<span data-ttu-id="4ec05-114">description</span><span class="sxs-lookup"><span data-stu-id="4ec05-114">description</span></span>|<span data-ttu-id="4ec05-115">String</span><span class="sxs-lookup"><span data-stu-id="4ec05-115">String</span></span>|<span data-ttu-id="4ec05-116">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="4ec05-116">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="4ec05-117">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="4ec05-117">securityIdentifier</span></span>|<span data-ttu-id="4ec05-118">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="4ec05-118">String</span></span>|<span data-ttu-id="4ec05-119">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="4ec05-119">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ec05-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4ec05-120">Relationships</span></span>
<span data-ttu-id="4ec05-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ec05-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ec05-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ec05-122">JSON Representation</span></span>
<span data-ttu-id="4ec05-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ec05-123">Here is a JSON representation of the resource.</span></span>
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



