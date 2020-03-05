---
title: tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd37bcb9dba4e4fc6ce54e686a6a889ce73448d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495169"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="603aa-103">tipo de recurso androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="603aa-103">androidEnrollmentCompanyCode resource type</span></span>

<span data-ttu-id="603aa-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="603aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="603aa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="603aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="603aa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="603aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="603aa-107">Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR</span><span class="sxs-lookup"><span data-stu-id="603aa-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="603aa-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="603aa-108">Properties</span></span>
|<span data-ttu-id="603aa-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="603aa-109">Property</span></span>|<span data-ttu-id="603aa-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="603aa-110">Type</span></span>|<span data-ttu-id="603aa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="603aa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="603aa-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="603aa-112">enrollmentToken</span></span>|<span data-ttu-id="603aa-113">String</span><span class="sxs-lookup"><span data-stu-id="603aa-113">String</span></span>|<span data-ttu-id="603aa-114">Token de registro usado pelo usuário para registrar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="603aa-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="603aa-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="603aa-115">qrCodeContent</span></span>|<span data-ttu-id="603aa-116">String</span><span class="sxs-lookup"><span data-stu-id="603aa-116">String</span></span>|<span data-ttu-id="603aa-117">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="603aa-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="603aa-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="603aa-118">qrCodeImage</span></span>|[<span data-ttu-id="603aa-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="603aa-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="603aa-120">Código QR gerado para o token.</span><span class="sxs-lookup"><span data-stu-id="603aa-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="603aa-121">Relações</span><span class="sxs-lookup"><span data-stu-id="603aa-121">Relationships</span></span>
<span data-ttu-id="603aa-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="603aa-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="603aa-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="603aa-123">JSON Representation</span></span>
<span data-ttu-id="603aa-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="603aa-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



