---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2a40fc3ab500fe6aa2a5b0f373c78524444b5bd1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971855"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="4699a-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="4699a-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="4699a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4699a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4699a-105">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="4699a-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="4699a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4699a-106">Properties</span></span>
|<span data-ttu-id="4699a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4699a-107">Property</span></span>|<span data-ttu-id="4699a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4699a-108">Type</span></span>|<span data-ttu-id="4699a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4699a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4699a-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="4699a-110">subjectName</span></span>|<span data-ttu-id="4699a-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4699a-111">String</span></span>|<span data-ttu-id="4699a-112">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4699a-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="4699a-113">descrição</span><span class="sxs-lookup"><span data-stu-id="4699a-113">description</span></span>|<span data-ttu-id="4699a-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4699a-114">String</span></span>|<span data-ttu-id="4699a-115">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4699a-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="4699a-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4699a-116">expirationDateTime</span></span>|<span data-ttu-id="4699a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4699a-117">DateTimeOffset</span></span>|<span data-ttu-id="4699a-118">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4699a-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="4699a-119">certificado</span><span class="sxs-lookup"><span data-stu-id="4699a-119">certificate</span></span>|<span data-ttu-id="4699a-120">Binário</span><span class="sxs-lookup"><span data-stu-id="4699a-120">Binary</span></span>|<span data-ttu-id="4699a-121">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="4699a-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="4699a-122">Relações</span><span class="sxs-lookup"><span data-stu-id="4699a-122">Relationships</span></span>
<span data-ttu-id="4699a-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4699a-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4699a-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4699a-124">JSON Representation</span></span>
<span data-ttu-id="4699a-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4699a-125">Here is a JSON representation of the resource.</span></span>
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



