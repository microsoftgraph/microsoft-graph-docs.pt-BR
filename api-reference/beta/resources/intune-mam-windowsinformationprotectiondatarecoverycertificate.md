---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 272a1e5f7bf1df1c9e16b2239caeee94cc81f12d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453992"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="1a1e6-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1a1e6-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="1a1e6-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a1e6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a1e6-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a1e6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a1e6-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="1a1e6-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="1a1e6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a1e6-107">Properties</span></span>
|<span data-ttu-id="1a1e6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a1e6-108">Property</span></span>|<span data-ttu-id="1a1e6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a1e6-109">Type</span></span>|<span data-ttu-id="1a1e6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a1e6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a1e6-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="1a1e6-111">subjectName</span></span>|<span data-ttu-id="1a1e6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1a1e6-112">String</span></span>|<span data-ttu-id="1a1e6-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1a1e6-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="1a1e6-114">description</span><span class="sxs-lookup"><span data-stu-id="1a1e6-114">description</span></span>|<span data-ttu-id="1a1e6-115">String</span><span class="sxs-lookup"><span data-stu-id="1a1e6-115">String</span></span>|<span data-ttu-id="1a1e6-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1a1e6-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="1a1e6-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a1e6-117">expirationDateTime</span></span>|<span data-ttu-id="1a1e6-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a1e6-118">DateTimeOffset</span></span>|<span data-ttu-id="1a1e6-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1a1e6-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="1a1e6-120">certificado</span><span class="sxs-lookup"><span data-stu-id="1a1e6-120">certificate</span></span>|<span data-ttu-id="1a1e6-121">Binário</span><span class="sxs-lookup"><span data-stu-id="1a1e6-121">Binary</span></span>|<span data-ttu-id="1a1e6-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1a1e6-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a1e6-123">Relações</span><span class="sxs-lookup"><span data-stu-id="1a1e6-123">Relationships</span></span>
<span data-ttu-id="1a1e6-124">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="1a1e6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a1e6-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a1e6-125">JSON Representation</span></span>
<span data-ttu-id="1a1e6-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a1e6-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





