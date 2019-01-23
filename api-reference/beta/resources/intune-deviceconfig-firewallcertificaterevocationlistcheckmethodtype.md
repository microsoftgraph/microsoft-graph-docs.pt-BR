---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4585c30c0a910befd8df8482636916af9ad9c0d6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396410"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="2cb53-103">tipo de enum firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="2cb53-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="2cb53-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="2cb53-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2cb53-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2cb53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2cb53-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="2cb53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cb53-107">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="2cb53-107">Possible values for firewallCertificateRevocationListCheckMethod</span></span>

## <a name="members"></a><span data-ttu-id="2cb53-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2cb53-108">Members</span></span>
|<span data-ttu-id="2cb53-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2cb53-109">Member</span></span>|<span data-ttu-id="2cb53-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2cb53-110">Value</span></span>|<span data-ttu-id="2cb53-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2cb53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2cb53-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="2cb53-112">deviceDefault</span></span>|<span data-ttu-id="2cb53-113">0</span><span class="sxs-lookup"><span data-stu-id="2cb53-113">0</span></span>|<span data-ttu-id="2cb53-114">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="2cb53-114">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="2cb53-115">none</span><span class="sxs-lookup"><span data-stu-id="2cb53-115">none</span></span>|<span data-ttu-id="2cb53-116">1</span><span class="sxs-lookup"><span data-stu-id="2cb53-116">1</span></span>|<span data-ttu-id="2cb53-117">Não verificar a lista de revogação de certificado</span><span class="sxs-lookup"><span data-stu-id="2cb53-117">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="2cb53-118">tentativa</span><span class="sxs-lookup"><span data-stu-id="2cb53-118">attempt</span></span>|<span data-ttu-id="2cb53-119">2</span><span class="sxs-lookup"><span data-stu-id="2cb53-119">2</span></span>|<span data-ttu-id="2cb53-120">Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de</span><span class="sxs-lookup"><span data-stu-id="2cb53-120">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="2cb53-121">exigir</span><span class="sxs-lookup"><span data-stu-id="2cb53-121">require</span></span>|<span data-ttu-id="2cb53-122">3</span><span class="sxs-lookup"><span data-stu-id="2cb53-122">3</span></span>|<span data-ttu-id="2cb53-123">Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado</span><span class="sxs-lookup"><span data-stu-id="2cb53-123">Require a successful CRL check before allowing a certificate</span></span>|




