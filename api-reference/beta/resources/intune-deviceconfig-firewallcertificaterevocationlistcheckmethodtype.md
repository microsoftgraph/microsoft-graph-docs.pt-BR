---
title: tipo de enumeração firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74989961978ddd10f2c14e57cfe31e25ac831703
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30170074"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="3e102-103">tipo de enumeração firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="3e102-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="3e102-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3e102-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e102-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3e102-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e102-106">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="3e102-106">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="3e102-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3e102-107">Members</span></span>
|<span data-ttu-id="3e102-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3e102-108">Member</span></span>|<span data-ttu-id="3e102-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3e102-109">Value</span></span>|<span data-ttu-id="3e102-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e102-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e102-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3e102-111">deviceDefault</span></span>|<span data-ttu-id="3e102-112">,0</span><span class="sxs-lookup"><span data-stu-id="3e102-112">0</span></span>|<span data-ttu-id="3e102-113">Nenhum valor configurado pelo Intune, não substitua o valor padrão do dispositivo configurado pelo usuário</span><span class="sxs-lookup"><span data-stu-id="3e102-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="3e102-114">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="3e102-114">none</span></span>|<span data-ttu-id="3e102-115">1</span><span class="sxs-lookup"><span data-stu-id="3e102-115">1</span></span>|<span data-ttu-id="3e102-116">Não verificar a lista de certificados revogados</span><span class="sxs-lookup"><span data-stu-id="3e102-116">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="3e102-117">Houve</span><span class="sxs-lookup"><span data-stu-id="3e102-117">attempt</span></span>|<span data-ttu-id="3e102-118">duas</span><span class="sxs-lookup"><span data-stu-id="3e102-118">2</span></span>|<span data-ttu-id="3e102-119">Tentar verificação de CRL e permitir um certificado somente se o certificado for confirmado pela verificação</span><span class="sxs-lookup"><span data-stu-id="3e102-119">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="3e102-120">precisa</span><span class="sxs-lookup"><span data-stu-id="3e102-120">require</span></span>|<span data-ttu-id="3e102-121">3D</span><span class="sxs-lookup"><span data-stu-id="3e102-121">3</span></span>|<span data-ttu-id="3e102-122">Exigir uma verificação de CRL bem-sucedida antes de permitir um certificado</span><span class="sxs-lookup"><span data-stu-id="3e102-122">Require a successful CRL check before allowing a certificate</span></span>|




