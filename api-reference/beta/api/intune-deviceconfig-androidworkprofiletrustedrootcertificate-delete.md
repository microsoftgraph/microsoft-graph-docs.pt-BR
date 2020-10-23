---
title: Excluir androidWorkProfileTrustedRootCertificate
description: Exclui androidWorkProfileTrustedRootCertificate.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 603dc1422e01c04b6b8d9864eebc2823f9b2e5db
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733850"
---
# <a name="delete-androidworkprofiletrustedrootcertificate"></a><span data-ttu-id="dc103-103">Excluir androidWorkProfileTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="dc103-103">Delete androidWorkProfileTrustedRootCertificate</span></span>

<span data-ttu-id="dc103-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc103-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dc103-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dc103-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc103-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dc103-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc103-107">Exclui [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="dc103-107">Deletes a [androidWorkProfileTrustedRootCertificate](../resources/intune-deviceconfig-androidworkprofiletrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dc103-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="dc103-108">Prerequisites</span></span>
<span data-ttu-id="dc103-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc103-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc103-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="dc103-111">Permission type</span></span>|<span data-ttu-id="dc103-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="dc103-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc103-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="dc103-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dc103-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc103-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc103-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="dc103-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc103-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="dc103-116">Not supported.</span></span>|
|<span data-ttu-id="dc103-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="dc103-117">Application</span></span>|<span data-ttu-id="dc103-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc103-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc103-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="dc103-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileCertificateProfileBase/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="dc103-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="dc103-120">Request headers</span></span>
|<span data-ttu-id="dc103-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="dc103-121">Header</span></span>|<span data-ttu-id="dc103-122">Valor</span><span class="sxs-lookup"><span data-stu-id="dc103-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc103-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="dc103-123">Authorization</span></span>|<span data-ttu-id="dc103-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dc103-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc103-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="dc103-125">Accept</span></span>|<span data-ttu-id="dc103-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dc103-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc103-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="dc103-127">Request body</span></span>
<span data-ttu-id="dc103-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="dc103-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc103-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc103-129">Response</span></span>
<span data-ttu-id="dc103-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="dc103-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="dc103-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="dc103-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="dc103-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="dc103-132">Request</span></span>
<span data-ttu-id="dc103-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="dc103-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
```

### <a name="response"></a><span data-ttu-id="dc103-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="dc103-134">Response</span></span>
<span data-ttu-id="dc103-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="dc103-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





