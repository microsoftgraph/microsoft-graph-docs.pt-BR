---
title: Tipo de recurso teamsDeviceUsageUserDetail
description: Representa detalhes sobre o uso de dispositivos do Microsoft Teams pelo usuário.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 294ffee8a1a5db208508cce230377285d6834b07
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766053"
---
# <a name="teamsdeviceusageuserdetail-resource-type"></a><span data-ttu-id="f6d96-103">Tipo de recurso teamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="f6d96-103">teamsDeviceUsageUserDetail resource type</span></span>

<span data-ttu-id="f6d96-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6d96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6d96-105">Representa detalhes sobre o uso de dispositivos do Microsoft Teams pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f6d96-105">Represents details about Microsoft Teams device usage by user.</span></span>

## <a name="properties"></a><span data-ttu-id="f6d96-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6d96-106">Properties</span></span>

| <span data-ttu-id="f6d96-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6d96-107">Property</span></span>          | <span data-ttu-id="f6d96-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6d96-108">Type</span></span>    | <span data-ttu-id="f6d96-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6d96-109">Description</span></span>                                                  |
| :---------------- | :------ | ------------------------------------------------------------ |
| <span data-ttu-id="f6d96-110">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="f6d96-110">reportRefreshDate</span></span> | <span data-ttu-id="f6d96-111">Data</span><span class="sxs-lookup"><span data-stu-id="f6d96-111">Date</span></span>    | <span data-ttu-id="f6d96-112">A data mais recente do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f6d96-112">The latest date of the content.</span></span>                              |
| <span data-ttu-id="f6d96-113">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f6d96-113">userPrincipalName</span></span> | <span data-ttu-id="f6d96-114">String</span><span class="sxs-lookup"><span data-stu-id="f6d96-114">String</span></span>  | <span data-ttu-id="f6d96-115">O nome UPN do usuário.</span><span class="sxs-lookup"><span data-stu-id="f6d96-115">The user principal name (UPN) of the user.</span></span> <span data-ttu-id="f6d96-116">O nome UPN é um nome de logon para o usuário ao estilo da Internet com base na RFC 822 padrão da Internet.</span><span class="sxs-lookup"><span data-stu-id="f6d96-116">The UPN is an Internet-style login name for the user based on the Internet standard RFC 822.</span></span> <span data-ttu-id="f6d96-117">Por convenção, ele deve ser mapeado para o nome de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="f6d96-117">By convention, this should map to the user's email name.</span></span> <span data-ttu-id="f6d96-118">O formato geral é alias@domain, em que o domínio deve estar presente na coleção de domínios verificados do locatário.</span><span class="sxs-lookup"><span data-stu-id="f6d96-118">The general format is alias@domain, where domain must be present in the tenant’s collection of verified domains.</span></span> <span data-ttu-id="f6d96-119">Essa propriedade é obrigatória quando um usuário é criado.</span><span class="sxs-lookup"><span data-stu-id="f6d96-119">This property is required when a user is created.</span></span> |
| <span data-ttu-id="f6d96-120">isLicensed</span><span class="sxs-lookup"><span data-stu-id="f6d96-120">isLicensed</span></span>        | <span data-ttu-id="f6d96-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-121">Boolean</span></span> | <span data-ttu-id="f6d96-122">Se o usuário recebeu uma licença do Teams.</span><span class="sxs-lookup"><span data-stu-id="f6d96-122">Whether the user has been assigned a Teams license.</span></span>          |
| <span data-ttu-id="f6d96-123">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="f6d96-123">lastActivityDate</span></span>  | <span data-ttu-id="f6d96-124">Data</span><span class="sxs-lookup"><span data-stu-id="f6d96-124">Date</span></span>    | <span data-ttu-id="f6d96-125">A última data em que o usuário participou de uma atividade do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f6d96-125">The last date that the user participated in a Microsoft Teams activity.</span></span> |
| <span data-ttu-id="f6d96-126">isDeleted</span><span class="sxs-lookup"><span data-stu-id="f6d96-126">isDeleted</span></span>         | <span data-ttu-id="f6d96-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-127">Boolean</span></span> | <span data-ttu-id="f6d96-128">Se esse usuário foi excluído ou excluído.</span><span class="sxs-lookup"><span data-stu-id="f6d96-128">Whether this user has been deleted or soft deleted.</span></span>          |
| <span data-ttu-id="f6d96-129">deletedDate</span><span class="sxs-lookup"><span data-stu-id="f6d96-129">deletedDate</span></span>       | <span data-ttu-id="f6d96-130">Data</span><span class="sxs-lookup"><span data-stu-id="f6d96-130">Date</span></span>    | <span data-ttu-id="f6d96-131">A data em que a operação de exclusão aconteceu.</span><span class="sxs-lookup"><span data-stu-id="f6d96-131">The date when the delete operation happened.</span></span> <span data-ttu-id="f6d96-132">O valor padrão é "null" quando o usuário não foi excluído.</span><span class="sxs-lookup"><span data-stu-id="f6d96-132">Default value is "null" when the user has not been deleted.</span></span> |
| <span data-ttu-id="f6d96-133">usedWeb</span><span class="sxs-lookup"><span data-stu-id="f6d96-133">usedWeb</span></span>           | <span data-ttu-id="f6d96-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-134">Boolean</span></span> | <span data-ttu-id="f6d96-135">Se o usuário estava ativo no cliente Web do Teams em dispositivos.</span><span class="sxs-lookup"><span data-stu-id="f6d96-135">Whether the user was active in the Teams web client on devices.</span></span> |
| <span data-ttu-id="f6d96-136">usedWindowsPhone</span><span class="sxs-lookup"><span data-stu-id="f6d96-136">usedWindowsPhone</span></span>  | <span data-ttu-id="f6d96-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-137">Boolean</span></span> | <span data-ttu-id="f6d96-138">Se o usuário estava ativo no cliente móvel do Teams para o telefone Windows.</span><span class="sxs-lookup"><span data-stu-id="f6d96-138">Whether the user was active on the Teams mobile client for Windows phone.</span></span> |
| <span data-ttu-id="f6d96-139">usediOS</span><span class="sxs-lookup"><span data-stu-id="f6d96-139">usediOS</span></span>           | <span data-ttu-id="f6d96-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-140">Boolean</span></span> | <span data-ttu-id="f6d96-141">Se o usuário estava ativo no cliente móvel do Teams para iOS.</span><span class="sxs-lookup"><span data-stu-id="f6d96-141">Whether the user was active on the Teams mobile client for iOS.</span></span> |
| <span data-ttu-id="f6d96-142">usedMac</span><span class="sxs-lookup"><span data-stu-id="f6d96-142">usedMac</span></span>           | <span data-ttu-id="f6d96-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-143">Boolean</span></span> | <span data-ttu-id="f6d96-144">Se o usuário estava ativo no cliente de área de trabalho do Teams em um computador macOS.</span><span class="sxs-lookup"><span data-stu-id="f6d96-144">Whether the user was active in the Teams desktop client on a macOS computer.</span></span> |
| <span data-ttu-id="f6d96-145">usedAndroidPhone</span><span class="sxs-lookup"><span data-stu-id="f6d96-145">usedAndroidPhone</span></span>  | <span data-ttu-id="f6d96-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-146">Boolean</span></span> | <span data-ttu-id="f6d96-147">Se o usuário estava ativo no cliente móvel do Teams para Android.</span><span class="sxs-lookup"><span data-stu-id="f6d96-147">Whether the user was active on the Teams mobile client for Android.</span></span> |
| <span data-ttu-id="f6d96-148">usedWindows</span><span class="sxs-lookup"><span data-stu-id="f6d96-148">usedWindows</span></span>       | <span data-ttu-id="f6d96-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-149">Boolean</span></span> | <span data-ttu-id="f6d96-150">Se o usuário estava ativo no cliente de área de trabalho do Teams em um computador baseado no Windows.</span><span class="sxs-lookup"><span data-stu-id="f6d96-150">Whether the user was active in the Teams desktop client on a Windows-based computer.</span></span> |
| <span data-ttu-id="f6d96-151">usedChromeOS</span><span class="sxs-lookup"><span data-stu-id="f6d96-151">usedChromeOS</span></span>      | <span data-ttu-id="f6d96-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-152">Boolean</span></span> | <span data-ttu-id="f6d96-153">Se o usuário estava ativo no cliente da área de trabalho do Teams em um computador ChromeOS.</span><span class="sxs-lookup"><span data-stu-id="f6d96-153">Whether the user was active in the Teams desktop client on a ChromeOS computer.</span></span> |
| <span data-ttu-id="f6d96-154">usedLinux</span><span class="sxs-lookup"><span data-stu-id="f6d96-154">usedLinux</span></span>         | <span data-ttu-id="f6d96-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6d96-155">Boolean</span></span> | <span data-ttu-id="f6d96-156">Se o usuário estava ativo no cliente de área de trabalho do Teams em um computador Linux.</span><span class="sxs-lookup"><span data-stu-id="f6d96-156">Whether the user was active in the Teams desktop client on a Linux computer.</span></span> |
| <span data-ttu-id="f6d96-157">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="f6d96-157">reportPeriod</span></span>      | <span data-ttu-id="f6d96-158">String</span><span class="sxs-lookup"><span data-stu-id="f6d96-158">String</span></span>  | <span data-ttu-id="f6d96-159">O número de dias que o relatório aborda.</span><span class="sxs-lookup"><span data-stu-id="f6d96-159">The number of days the report covers.</span></span>                        |

## <a name="json-representation"></a><span data-ttu-id="f6d96-160">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6d96-160">JSON representation</span></span>

<span data-ttu-id="f6d96-161">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6d96-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "isLicensed": true, 
  "lastActivityDate": "Date", 
  "isDeleted": true, 
  "deletedDate": "Date", 
  "usedWeb": true, 
  "usedWindowsPhone": true, 
  "usediOS": true, 
  "usedMac": true, 
  "usedAndroidPhone": true, 
  "usedWindows": true, 
  "usedChromeOS": true, 
  "usedLinux": true, 
  "reportPeriod": "String"
}
```


