---
title: tipo de enumeração emailCertificateType
description: Fontes de certificado com suporte para assinatura e criptografia de email.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2ff58f55033660a839a5f28d0244217c62936e0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996383"
---
# <a name="emailcertificatetype-enum-type"></a><span data-ttu-id="a06f7-103">tipo de enumeração emailCertificateType</span><span class="sxs-lookup"><span data-stu-id="a06f7-103">emailCertificateType enum type</span></span>

> <span data-ttu-id="a06f7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a06f7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a06f7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a06f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a06f7-106">Fontes de certificado com suporte para assinatura e criptografia de email.</span><span class="sxs-lookup"><span data-stu-id="a06f7-106">Supported certificate sources for email signing and encryption.</span></span>

## <a name="members"></a><span data-ttu-id="a06f7-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a06f7-107">Members</span></span>
|<span data-ttu-id="a06f7-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a06f7-108">Member</span></span>|<span data-ttu-id="a06f7-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a06f7-109">Value</span></span>|<span data-ttu-id="a06f7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a06f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a06f7-111">none</span><span class="sxs-lookup"><span data-stu-id="a06f7-111">none</span></span>|<span data-ttu-id="a06f7-112">,0</span><span class="sxs-lookup"><span data-stu-id="a06f7-112">0</span></span>|<span data-ttu-id="a06f7-113">Não use um certificado como fonte.</span><span class="sxs-lookup"><span data-stu-id="a06f7-113">Do not use a certificate as a source.</span></span>|
|<span data-ttu-id="a06f7-114">certificado</span><span class="sxs-lookup"><span data-stu-id="a06f7-114">certificate</span></span>|<span data-ttu-id="a06f7-115">1</span><span class="sxs-lookup"><span data-stu-id="a06f7-115">1</span></span>|<span data-ttu-id="a06f7-116">Usar um certificado para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="a06f7-116">Use an certificate for certificate source.</span></span>|
|<span data-ttu-id="a06f7-117">derivedCredential</span><span class="sxs-lookup"><span data-stu-id="a06f7-117">derivedCredential</span></span>|<span data-ttu-id="a06f7-118">duas</span><span class="sxs-lookup"><span data-stu-id="a06f7-118">2</span></span>|<span data-ttu-id="a06f7-119">Use uma credencial derivada para a fonte do certificado.</span><span class="sxs-lookup"><span data-stu-id="a06f7-119">Use a derived credential for certificate source.</span></span>|





