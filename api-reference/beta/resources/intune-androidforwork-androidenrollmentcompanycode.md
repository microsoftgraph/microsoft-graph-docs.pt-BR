---
title: tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0422bf09d990c02c984b45fa144d6ae12661f718
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552788"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="76ef5-103">tipo de recurso androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="76ef5-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="76ef5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="76ef5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76ef5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76ef5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76ef5-106">Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR</span><span class="sxs-lookup"><span data-stu-id="76ef5-106">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="76ef5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76ef5-107">Properties</span></span>
|<span data-ttu-id="76ef5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76ef5-108">Property</span></span>|<span data-ttu-id="76ef5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="76ef5-109">Type</span></span>|<span data-ttu-id="76ef5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76ef5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76ef5-111">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="76ef5-111">enrollmentToken</span></span>|<span data-ttu-id="76ef5-112">String</span><span class="sxs-lookup"><span data-stu-id="76ef5-112">String</span></span>|<span data-ttu-id="76ef5-113">Token de registro usado pelo usuário para registrar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="76ef5-113">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="76ef5-114">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="76ef5-114">qrCodeContent</span></span>|<span data-ttu-id="76ef5-115">String</span><span class="sxs-lookup"><span data-stu-id="76ef5-115">String</span></span>|<span data-ttu-id="76ef5-116">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="76ef5-116">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="76ef5-117">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="76ef5-117">qrCodeImage</span></span>|[<span data-ttu-id="76ef5-118">mimeContent</span><span class="sxs-lookup"><span data-stu-id="76ef5-118">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="76ef5-119">Código QR gerado para o token.</span><span class="sxs-lookup"><span data-stu-id="76ef5-119">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76ef5-120">Relações</span><span class="sxs-lookup"><span data-stu-id="76ef5-120">Relationships</span></span>
<span data-ttu-id="76ef5-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76ef5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76ef5-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76ef5-122">JSON Representation</span></span>
<span data-ttu-id="76ef5-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76ef5-123">Here is a JSON representation of the resource.</span></span>
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





