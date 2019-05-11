---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92d0f13416e543e018a5a69d28751d9ddd4512c8
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946634"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="d449a-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="d449a-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="d449a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d449a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d449a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d449a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d449a-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="d449a-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="d449a-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d449a-107">Members</span></span>
|<span data-ttu-id="d449a-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d449a-108">Member</span></span>|<span data-ttu-id="d449a-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d449a-109">Value</span></span>|<span data-ttu-id="d449a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d449a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d449a-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d449a-111">deviceDefault</span></span>|<span data-ttu-id="d449a-112">,0</span><span class="sxs-lookup"><span data-stu-id="d449a-112">0</span></span>|<span data-ttu-id="d449a-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="d449a-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="d449a-114">none</span><span class="sxs-lookup"><span data-stu-id="d449a-114">none</span></span>|<span data-ttu-id="d449a-115">1</span><span class="sxs-lookup"><span data-stu-id="d449a-115">1</span></span>|<span data-ttu-id="d449a-116">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="d449a-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="d449a-117">Houve</span><span class="sxs-lookup"><span data-stu-id="d449a-117">attempt</span></span>|<span data-ttu-id="d449a-118">duas</span><span class="sxs-lookup"><span data-stu-id="d449a-118">2</span></span>|<span data-ttu-id="d449a-119">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="d449a-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="d449a-120">precisa</span><span class="sxs-lookup"><span data-stu-id="d449a-120">require</span></span>|<span data-ttu-id="d449a-121">3D</span><span class="sxs-lookup"><span data-stu-id="d449a-121">3</span></span>|<span data-ttu-id="d449a-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="d449a-122">Require a successful CRL check before allowing a certificate</span></span>|




