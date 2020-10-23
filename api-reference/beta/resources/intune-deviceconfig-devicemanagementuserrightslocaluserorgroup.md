---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cf4d5ebcd77dfef119d97e0d5bbe2bfbfb93c4e7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707812"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="2b98b-103">tipo de recurso deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="2b98b-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

<span data-ttu-id="2b98b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b98b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b98b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b98b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b98b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b98b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b98b-107">Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.</span><span class="sxs-lookup"><span data-stu-id="2b98b-107">Represents information for a local user or group used for user rights setting.</span></span>

## <a name="properties"></a><span data-ttu-id="2b98b-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b98b-108">Properties</span></span>
|<span data-ttu-id="2b98b-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b98b-109">Property</span></span>|<span data-ttu-id="2b98b-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b98b-110">Type</span></span>|<span data-ttu-id="2b98b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b98b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b98b-112">nome</span><span class="sxs-lookup"><span data-stu-id="2b98b-112">name</span></span>|<span data-ttu-id="2b98b-113">String</span><span class="sxs-lookup"><span data-stu-id="2b98b-113">String</span></span>|<span data-ttu-id="2b98b-114">O nome desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="2b98b-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="2b98b-115">description</span><span class="sxs-lookup"><span data-stu-id="2b98b-115">description</span></span>|<span data-ttu-id="2b98b-116">String</span><span class="sxs-lookup"><span data-stu-id="2b98b-116">String</span></span>|<span data-ttu-id="2b98b-117">Descrição do administrador desse usuário ou grupo local.</span><span class="sxs-lookup"><span data-stu-id="2b98b-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="2b98b-118">securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="2b98b-118">securityIdentifier</span></span>|<span data-ttu-id="2b98b-119">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="2b98b-119">String</span></span>|<span data-ttu-id="2b98b-120">O identificador de segurança desse usuário ou grupo local (por exemplo, \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="2b98b-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b98b-121">Relações</span><span class="sxs-lookup"><span data-stu-id="2b98b-121">Relationships</span></span>
<span data-ttu-id="2b98b-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b98b-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b98b-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b98b-123">JSON Representation</span></span>
<span data-ttu-id="2b98b-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b98b-124">Here is a JSON representation of the resource.</span></span>
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





