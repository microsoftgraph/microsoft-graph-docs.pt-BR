---
title: Ação enableUnlicensedAdminstrators
description: Após a habilitação, os usuários atribuídos como administradores por meio de Associações de Atribuição de Função não exigirão mais uma licença atribuída do Intune. Você está limitado a 350 membros diretos sem licença para cada grupo de segurança do AAD em uma atribuição de função, mas pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenças. Os administradores licenciados continuarão a funcionar como estão na medida em que as associações transitivas se aplicam e não estão sujeitas ao limite de 350 membros.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 149c14aab5672939174799791f6a4e0af970419d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51128023"
---
# <a name="enableunlicensedadminstrators-action"></a><span data-ttu-id="e5777-105">Ação enableUnlicensedAdminstrators</span><span class="sxs-lookup"><span data-stu-id="e5777-105">enableUnlicensedAdminstrators action</span></span>

<span data-ttu-id="e5777-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5777-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e5777-107">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e5777-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5777-108">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e5777-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5777-109">Após a habilitação, os usuários atribuídos como administradores por meio de Associações de Atribuição de Função não exigirão mais uma licença atribuída do Intune.</span><span class="sxs-lookup"><span data-stu-id="e5777-109">Upon enabling, users assigned as administrators via Role Assignment Memberships will no longer require an assigned Intune license.</span></span> <span data-ttu-id="e5777-110">Você está limitado a 350 membros diretos sem licença para cada grupo de segurança do AAD em uma atribuição de função, mas pode atribuir vários grupos de segurança do AAD a uma função se precisar dar suporte a mais de 350 administradores não licenças.</span><span class="sxs-lookup"><span data-stu-id="e5777-110">You are limited to 350 unlicensed direct members for each AAD security group in a role assignment, but you can assign multiple AAD security groups to a role if you need to support more than 350 unlicensed administrators.</span></span> <span data-ttu-id="e5777-111">Os administradores licenciados continuarão a funcionar como estão na medida em que as associações transitivas se aplicam e não estão sujeitas ao limite de 350 membros.</span><span class="sxs-lookup"><span data-stu-id="e5777-111">Licensed administrators will continue to function as-is in that transitive memberships apply and are not subject to the 350 member limit.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e5777-112">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5777-112">Prerequisites</span></span>
<span data-ttu-id="e5777-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5777-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5777-115">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5777-115">Permission type</span></span>|<span data-ttu-id="e5777-116">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e5777-116">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5777-117">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5777-117">Delegated (work or school account)</span></span>|<span data-ttu-id="e5777-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5777-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e5777-119">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5777-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5777-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5777-120">Not supported.</span></span>|
|<span data-ttu-id="e5777-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5777-121">Application</span></span>|<span data-ttu-id="e5777-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5777-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5777-123">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5777-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a><span data-ttu-id="e5777-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5777-124">Request headers</span></span>
|<span data-ttu-id="e5777-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5777-125">Header</span></span>|<span data-ttu-id="e5777-126">Valor</span><span class="sxs-lookup"><span data-stu-id="e5777-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5777-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5777-127">Authorization</span></span>|<span data-ttu-id="e5777-128">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5777-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5777-129">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5777-129">Accept</span></span>|<span data-ttu-id="e5777-130">application/json</span><span class="sxs-lookup"><span data-stu-id="e5777-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5777-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5777-131">Request body</span></span>
<span data-ttu-id="e5777-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e5777-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5777-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5777-133">Response</span></span>
<span data-ttu-id="e5777-134">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e5777-134">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e5777-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5777-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="e5777-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5777-136">Request</span></span>
<span data-ttu-id="e5777-137">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5777-137">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a><span data-ttu-id="e5777-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5777-138">Response</span></span>
<span data-ttu-id="e5777-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5777-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




