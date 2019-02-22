---
title: Excluir iosPkcsCertificateProfile
description: Exclui iosPkcsCertificateProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8949d6f50f08dc818c8ff103e4bf930704c0ba33
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139876"
---
# <a name="delete-iospkcscertificateprofile"></a><span data-ttu-id="2eb98-103">Excluir iosPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2eb98-103">Delete iosPkcsCertificateProfile</span></span>

> <span data-ttu-id="2eb98-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2eb98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2eb98-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2eb98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2eb98-106">Exclui [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span><span class="sxs-lookup"><span data-stu-id="2eb98-106">Deletes a [iosPkcsCertificateProfile](../resources/intune-deviceconfig-iospkcscertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2eb98-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2eb98-107">Prerequisites</span></span>
<span data-ttu-id="2eb98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2eb98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2eb98-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2eb98-110">Permission type</span></span>|<span data-ttu-id="2eb98-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2eb98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2eb98-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2eb98-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2eb98-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2eb98-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2eb98-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2eb98-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2eb98-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb98-115">Not supported.</span></span>|
|<span data-ttu-id="2eb98-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2eb98-116">Application</span></span>|<span data-ttu-id="2eb98-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2eb98-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2eb98-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2eb98-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2eb98-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb98-119">Request headers</span></span>
|<span data-ttu-id="2eb98-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2eb98-120">Header</span></span>|<span data-ttu-id="2eb98-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2eb98-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2eb98-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2eb98-122">Authorization</span></span>|<span data-ttu-id="2eb98-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2eb98-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2eb98-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2eb98-124">Accept</span></span>|<span data-ttu-id="2eb98-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2eb98-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2eb98-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb98-126">Request body</span></span>
<span data-ttu-id="2eb98-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2eb98-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2eb98-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb98-128">Response</span></span>
<span data-ttu-id="2eb98-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2eb98-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2eb98-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2eb98-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2eb98-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2eb98-131">Request</span></span>
<span data-ttu-id="2eb98-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2eb98-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2eb98-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2eb98-133">Response</span></span>
<span data-ttu-id="2eb98-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2eb98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




