---
title: tipo de recurso managementCertificateWithThumbprint
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 45a8544f9c032c386f99caa2f8d174d495673c29
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43460719"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="2d03a-103">tipo de recurso managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="2d03a-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="2d03a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d03a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d03a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d03a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d03a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d03a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d03a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2d03a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2d03a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2d03a-108">Properties</span></span>
|<span data-ttu-id="2d03a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2d03a-109">Property</span></span>|<span data-ttu-id="2d03a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2d03a-110">Type</span></span>|<span data-ttu-id="2d03a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d03a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d03a-112">identificação</span><span class="sxs-lookup"><span data-stu-id="2d03a-112">thumbprint</span></span>|<span data-ttu-id="2d03a-113">String</span><span class="sxs-lookup"><span data-stu-id="2d03a-113">String</span></span>|<span data-ttu-id="2d03a-114">A impressão digital do certificado de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="2d03a-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="2d03a-115">certificado</span><span class="sxs-lookup"><span data-stu-id="2d03a-115">certificate</span></span>|<span data-ttu-id="2d03a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2d03a-116">String</span></span>|<span data-ttu-id="2d03a-117">O certificado de gerenciamento codificado base 64</span><span class="sxs-lookup"><span data-stu-id="2d03a-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d03a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="2d03a-118">Relationships</span></span>
<span data-ttu-id="2d03a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2d03a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d03a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2d03a-120">JSON Representation</span></span>
<span data-ttu-id="2d03a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2d03a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```



