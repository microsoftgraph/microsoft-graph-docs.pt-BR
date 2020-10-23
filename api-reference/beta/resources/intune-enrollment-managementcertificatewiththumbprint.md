---
title: tipo de recurso managementCertificateWithThumbprint
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5fee7a35e20461cec2fba40b34273d0d947416e1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728953"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="3d58a-103">tipo de recurso managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="3d58a-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="3d58a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d58a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d58a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3d58a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d58a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3d58a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d58a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3d58a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3d58a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d58a-108">Properties</span></span>
|<span data-ttu-id="3d58a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d58a-109">Property</span></span>|<span data-ttu-id="3d58a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d58a-110">Type</span></span>|<span data-ttu-id="3d58a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d58a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d58a-112">identificação</span><span class="sxs-lookup"><span data-stu-id="3d58a-112">thumbprint</span></span>|<span data-ttu-id="3d58a-113">String</span><span class="sxs-lookup"><span data-stu-id="3d58a-113">String</span></span>|<span data-ttu-id="3d58a-114">A impressão digital do certificado de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="3d58a-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="3d58a-115">certificado</span><span class="sxs-lookup"><span data-stu-id="3d58a-115">certificate</span></span>|<span data-ttu-id="3d58a-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3d58a-116">String</span></span>|<span data-ttu-id="3d58a-117">O certificado de gerenciamento codificado base 64</span><span class="sxs-lookup"><span data-stu-id="3d58a-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d58a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3d58a-118">Relationships</span></span>
<span data-ttu-id="3d58a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d58a-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d58a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d58a-120">JSON Representation</span></span>
<span data-ttu-id="3d58a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d58a-121">Here is a JSON representation of the resource.</span></span>
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





