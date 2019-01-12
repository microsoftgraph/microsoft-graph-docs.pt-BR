---
title: tipo de enum firewallCertificateRevocationListCheckMethodType
description: Valores possíveis para firewallCertificateRevocationListCheckMethod
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e479b10339ab515a17f67d85de0c8d43c1507825
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940054"
---
# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="f437a-103">tipo de enum firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="f437a-103">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="f437a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f437a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f437a-105">Valores possíveis para firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="f437a-105">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="f437a-106">Membros</span><span class="sxs-lookup"><span data-stu-id="f437a-106">Members</span></span>
|<span data-ttu-id="f437a-107">Membro</span><span class="sxs-lookup"><span data-stu-id="f437a-107">Member</span></span>|<span data-ttu-id="f437a-108">Valor</span><span class="sxs-lookup"><span data-stu-id="f437a-108">Value</span></span>|<span data-ttu-id="f437a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f437a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f437a-110">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f437a-110">deviceDefault</span></span>|<span data-ttu-id="f437a-111">0</span><span class="sxs-lookup"><span data-stu-id="f437a-111">0</span></span>|<span data-ttu-id="f437a-112">Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário</span><span class="sxs-lookup"><span data-stu-id="f437a-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f437a-113">nenhum</span><span class="sxs-lookup"><span data-stu-id="f437a-113">none</span></span>|<span data-ttu-id="f437a-114">1</span><span class="sxs-lookup"><span data-stu-id="f437a-114">1</span></span>|<span data-ttu-id="f437a-115">Não verificar a lista de revogação de certificado</span><span class="sxs-lookup"><span data-stu-id="f437a-115">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="f437a-116">tentativa</span><span class="sxs-lookup"><span data-stu-id="f437a-116">attempt</span></span>|<span data-ttu-id="f437a-117">2</span><span class="sxs-lookup"><span data-stu-id="f437a-117">2</span></span>|<span data-ttu-id="f437a-118">Tente verificação CRL e permitir que um certificado somente se o certificado for confirmado pela verificação de</span><span class="sxs-lookup"><span data-stu-id="f437a-118">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="f437a-119">exigir</span><span class="sxs-lookup"><span data-stu-id="f437a-119">require</span></span>|<span data-ttu-id="f437a-120">3</span><span class="sxs-lookup"><span data-stu-id="f437a-120">3</span></span>|<span data-ttu-id="f437a-121">Exigir uma verificação CRL bem-sucedida antes de permitir que um certificado</span><span class="sxs-lookup"><span data-stu-id="f437a-121">Require a successful CRL check before allowing a certificate</span></span>|



