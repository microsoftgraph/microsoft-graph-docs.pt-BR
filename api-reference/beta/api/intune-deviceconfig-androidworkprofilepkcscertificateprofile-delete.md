---
title: Excluir androidWorkProfilePkcsCertificateProfile
description: Exclui androidWorkProfilePkcsCertificateProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 47ca98da6b96c406f58018a862502ab93952ffb2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078959"
---
# <a name="delete-androidworkprofilepkcscertificateprofile"></a><span data-ttu-id="6ec95-103">Excluir androidWorkProfilePkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="6ec95-103">Delete androidWorkProfilePkcsCertificateProfile</span></span>

<span data-ttu-id="6ec95-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ec95-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ec95-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ec95-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec95-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ec95-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec95-107">Exclui [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6ec95-107">Deletes a [androidWorkProfilePkcsCertificateProfile](../resources/intune-deviceconfig-androidworkprofilepkcscertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ec95-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ec95-108">Prerequisites</span></span>
<span data-ttu-id="6ec95-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ec95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ec95-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ec95-111">Permission type</span></span>|<span data-ttu-id="6ec95-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ec95-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ec95-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ec95-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ec95-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ec95-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ec95-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ec95-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ec95-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ec95-116">Not supported.</span></span>|
|<span data-ttu-id="6ec95-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ec95-117">Application</span></span>|<span data-ttu-id="6ec95-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ec95-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ec95-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ec95-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6ec95-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ec95-120">Request headers</span></span>
|<span data-ttu-id="6ec95-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ec95-121">Header</span></span>|<span data-ttu-id="6ec95-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ec95-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ec95-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ec95-123">Authorization</span></span>|<span data-ttu-id="6ec95-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ec95-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ec95-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ec95-125">Accept</span></span>|<span data-ttu-id="6ec95-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ec95-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ec95-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ec95-127">Request body</span></span>
<span data-ttu-id="6ec95-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6ec95-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ec95-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ec95-129">Response</span></span>
<span data-ttu-id="6ec95-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="6ec95-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6ec95-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ec95-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ec95-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ec95-132">Request</span></span>
<span data-ttu-id="6ec95-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ec95-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6ec95-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ec95-134">Response</span></span>
<span data-ttu-id="6ec95-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ec95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






