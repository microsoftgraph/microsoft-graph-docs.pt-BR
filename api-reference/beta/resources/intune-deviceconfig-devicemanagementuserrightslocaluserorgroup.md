---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a4e935781bf0524f5fb5df2a8a9ecd868767bfed
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530114"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="c653e-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="c653e-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="c653e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c653e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c653e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c653e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c653e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c653e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c653e-107">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="c653e-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="c653e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c653e-108">Properties</span></span>
|<span data-ttu-id="c653e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c653e-109">Property</span></span>|<span data-ttu-id="c653e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c653e-110">Type</span></span>|<span data-ttu-id="c653e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c653e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c653e-112">nome</span><span class="sxs-lookup"><span data-stu-id="c653e-112">name</span></span>|<span data-ttu-id="c653e-113">String</span><span class="sxs-lookup"><span data-stu-id="c653e-113">String</span></span>|<span data-ttu-id="c653e-114">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="c653e-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="c653e-115">description</span><span class="sxs-lookup"><span data-stu-id="c653e-115">description</span></span>|<span data-ttu-id="c653e-116">String</span><span class="sxs-lookup"><span data-stu-id="c653e-116">String</span></span>|<span data-ttu-id="c653e-117">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="c653e-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="c653e-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="c653e-118">securityIdentifier</span></span>|<span data-ttu-id="c653e-119">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="c653e-119">String</span></span>|<span data-ttu-id="c653e-120">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="c653e-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c653e-121">Relações</span><span class="sxs-lookup"><span data-stu-id="c653e-121">Relationships</span></span>
<span data-ttu-id="c653e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c653e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c653e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c653e-123">JSON Representation</span></span>
<span data-ttu-id="c653e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c653e-124">Here is a JSON representation of the resource.</span></span>
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



