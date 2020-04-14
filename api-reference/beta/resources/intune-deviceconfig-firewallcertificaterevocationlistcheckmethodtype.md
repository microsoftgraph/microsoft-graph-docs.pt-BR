---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f220d5e592544ec3527c16c425d4b22fe0266d4c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43444306"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="29cc3-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="29cc3-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

<span data-ttu-id="29cc3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29cc3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29cc3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="29cc3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29cc3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="29cc3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29cc3-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="29cc3-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="29cc3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="29cc3-108">Members</span></span>
|<span data-ttu-id="29cc3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="29cc3-109">Member</span></span>|<span data-ttu-id="29cc3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="29cc3-110">Value</span></span>|<span data-ttu-id="29cc3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="29cc3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29cc3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="29cc3-112">deviceDefault</span></span>|<span data-ttu-id="29cc3-113">,0</span><span class="sxs-lookup"><span data-stu-id="29cc3-113">0</span></span>|<span data-ttu-id="29cc3-114">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="29cc3-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="29cc3-115">nenhuma</span><span class="sxs-lookup"><span data-stu-id="29cc3-115">none</span></span>|<span data-ttu-id="29cc3-116">1</span><span class="sxs-lookup"><span data-stu-id="29cc3-116">1</span></span>|<span data-ttu-id="29cc3-117">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="29cc3-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="29cc3-118">Houve</span><span class="sxs-lookup"><span data-stu-id="29cc3-118">attempt</span></span>|<span data-ttu-id="29cc3-119">duas</span><span class="sxs-lookup"><span data-stu-id="29cc3-119">2</span></span>|<span data-ttu-id="29cc3-120">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="29cc3-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="29cc3-121">precisa</span><span class="sxs-lookup"><span data-stu-id="29cc3-121">require</span></span>|<span data-ttu-id="29cc3-122">3D</span><span class="sxs-lookup"><span data-stu-id="29cc3-122">3</span></span>|<span data-ttu-id="29cc3-123">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="29cc3-123">Require a successful CRL check before allowing a certificate</span></span>|



