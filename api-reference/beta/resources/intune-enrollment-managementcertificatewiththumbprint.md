---
title: tipo de recurso managementCertificateWithThumbprint
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9fc6535147b8e7a5f2a2295b09cb73cce86c1793
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327805"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="2cd87-103">tipo de recurso managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="2cd87-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="2cd87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2cd87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cd87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2cd87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cd87-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2cd87-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2cd87-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2cd87-107">Properties</span></span>
|<span data-ttu-id="2cd87-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2cd87-108">Property</span></span>|<span data-ttu-id="2cd87-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2cd87-109">Type</span></span>|<span data-ttu-id="2cd87-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cd87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cd87-111">identificação</span><span class="sxs-lookup"><span data-stu-id="2cd87-111">thumbprint</span></span>|<span data-ttu-id="2cd87-112">String</span><span class="sxs-lookup"><span data-stu-id="2cd87-112">String</span></span>|<span data-ttu-id="2cd87-113">A impressão digital do certificado de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="2cd87-113">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="2cd87-114">certificado</span><span class="sxs-lookup"><span data-stu-id="2cd87-114">certificate</span></span>|<span data-ttu-id="2cd87-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2cd87-115">String</span></span>|<span data-ttu-id="2cd87-116">O certificado de gerenciamento codificado base 64</span><span class="sxs-lookup"><span data-stu-id="2cd87-116">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="2cd87-117">Relações</span><span class="sxs-lookup"><span data-stu-id="2cd87-117">Relationships</span></span>
<span data-ttu-id="2cd87-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cd87-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cd87-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2cd87-119">JSON Representation</span></span>
<span data-ttu-id="2cd87-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2cd87-120">Here is a JSON representation of the resource.</span></span>
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



