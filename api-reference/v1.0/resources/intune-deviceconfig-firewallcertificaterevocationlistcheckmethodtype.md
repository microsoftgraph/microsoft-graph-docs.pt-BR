---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a475f32d4572b0aa8ed2a52befc7a58eb6077253
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257628"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="76c53-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="76c53-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="76c53-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76c53-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76c53-105">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="76c53-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="76c53-106">Membros</span><span class="sxs-lookup"><span data-stu-id="76c53-106">Members</span></span>
|<span data-ttu-id="76c53-107">Membro</span><span class="sxs-lookup"><span data-stu-id="76c53-107">Member</span></span>|<span data-ttu-id="76c53-108">Valor</span><span class="sxs-lookup"><span data-stu-id="76c53-108">Value</span></span>|<span data-ttu-id="76c53-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="76c53-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76c53-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="76c53-110">deviceDefault</span></span>|<span data-ttu-id="76c53-111">,0</span><span class="sxs-lookup"><span data-stu-id="76c53-111">0</span></span>|<span data-ttu-id="76c53-112">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="76c53-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="76c53-113">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="76c53-113">none</span></span>|<span data-ttu-id="76c53-114">1</span><span class="sxs-lookup"><span data-stu-id="76c53-114">1</span></span>|<span data-ttu-id="76c53-115">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="76c53-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="76c53-116">Houve</span><span class="sxs-lookup"><span data-stu-id="76c53-116">attempt</span></span>|<span data-ttu-id="76c53-117">duas</span><span class="sxs-lookup"><span data-stu-id="76c53-117">2</span></span>|<span data-ttu-id="76c53-118">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="76c53-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="76c53-119">precisa</span><span class="sxs-lookup"><span data-stu-id="76c53-119">require</span></span>|<span data-ttu-id="76c53-120">3D</span><span class="sxs-lookup"><span data-stu-id="76c53-120">3</span></span>|<span data-ttu-id="76c53-121">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="76c53-121">Require a successful CRL check before allowing a certificate</span></span>|



