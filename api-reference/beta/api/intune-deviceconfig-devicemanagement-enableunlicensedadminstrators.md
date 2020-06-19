---
title: ação enableUnlicensedAdminstrators
description: Após a habilitação, os usuários atribuídos como administradores por meio de associações de atribuição de função não precisarão mais de uma licença do Intune atribuída. Você está limitado a 350 membros diretos não licenciados para cada grupo de segurança do AAD em uma atribuição de função, mas você pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenciados. Os administradores licenciados continuarão a funcionar como estão, já que as associações transitivas se aplicam e não estão sujeitas ao limite de membro de 350.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 882a5d1cafa8e25d4a69a0c525c0bb8d3b971cd1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792803"
---
# <a name="enableunlicensedadminstrators-action"></a><span data-ttu-id="353a4-105">ação enableUnlicensedAdminstrators</span><span class="sxs-lookup"><span data-stu-id="353a4-105">enableUnlicensedAdminstrators action</span></span>

<span data-ttu-id="353a4-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="353a4-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="353a4-107">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="353a4-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="353a4-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="353a4-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="353a4-109">Após a habilitação, os usuários atribuídos como administradores por meio de associações de atribuição de função não precisarão mais de uma licença do Intune atribuída.</span><span class="sxs-lookup"><span data-stu-id="353a4-109">Upon enabling, users assigned as administrators via Role Assignment Memberships will no longer require an assigned Intune license.</span></span> <span data-ttu-id="353a4-110">Você está limitado a 350 membros diretos não licenciados para cada grupo de segurança do AAD em uma atribuição de função, mas você pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenciados.</span><span class="sxs-lookup"><span data-stu-id="353a4-110">You are limited to 350 unlicensed direct members for each AAD security group in a role assignment, but you can assign multiple AAD security groups to a role if you need to support more than 350 unlicensed administrators.</span></span> <span data-ttu-id="353a4-111">Os administradores licenciados continuarão a funcionar como estão, já que as associações transitivas se aplicam e não estão sujeitas ao limite de membro de 350.</span><span class="sxs-lookup"><span data-stu-id="353a4-111">Licensed administrators will continue to function as-is in that transitive memberships apply and are not subject to the 350 member limit.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="353a4-112">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="353a4-112">Prerequisites</span></span>
<span data-ttu-id="353a4-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="353a4-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="353a4-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="353a4-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="353a4-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="353a4-115">Permission type</span></span>|<span data-ttu-id="353a4-116">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="353a4-116">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="353a4-117">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="353a4-117">Delegated (work or school account)</span></span>|<span data-ttu-id="353a4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="353a4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="353a4-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="353a4-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="353a4-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="353a4-120">Not supported.</span></span>|
|<span data-ttu-id="353a4-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="353a4-121">Application</span></span>|<span data-ttu-id="353a4-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="353a4-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="353a4-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="353a4-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a><span data-ttu-id="353a4-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="353a4-124">Request headers</span></span>
|<span data-ttu-id="353a4-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="353a4-125">Header</span></span>|<span data-ttu-id="353a4-126">Valor</span><span class="sxs-lookup"><span data-stu-id="353a4-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="353a4-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="353a4-127">Authorization</span></span>|<span data-ttu-id="353a4-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="353a4-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="353a4-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="353a4-129">Accept</span></span>|<span data-ttu-id="353a4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="353a4-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="353a4-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="353a4-131">Request body</span></span>
<span data-ttu-id="353a4-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="353a4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="353a4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="353a4-133">Response</span></span>
<span data-ttu-id="353a4-134">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="353a4-134">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="353a4-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="353a4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="353a4-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="353a4-136">Request</span></span>
<span data-ttu-id="353a4-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="353a4-137">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a><span data-ttu-id="353a4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="353a4-138">Response</span></span>
<span data-ttu-id="353a4-139">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="353a4-139">Here is an example of the response.</span></span> <span data-ttu-id="353a4-140">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="353a4-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="353a4-141">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="353a4-141">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



