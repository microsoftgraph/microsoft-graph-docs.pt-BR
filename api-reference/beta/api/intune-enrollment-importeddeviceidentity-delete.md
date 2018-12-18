---
title: Excluir importedDeviceIdentity
description: Exclui um importedDeviceIdentity.
author: tfitzmac
ms.openlocfilehash: e747e2331f12792c278a1bdc717527ff3222413d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338133"
---
# <a name="delete-importeddeviceidentity"></a><span data-ttu-id="b0e41-103">Excluir importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="b0e41-103">Delete importedDeviceIdentity</span></span>

> <span data-ttu-id="b0e41-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b0e41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b0e41-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b0e41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0e41-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b0e41-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0e41-107">Exclui um [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span><span class="sxs-lookup"><span data-stu-id="b0e41-107">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0e41-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b0e41-108">Prerequisites</span></span>
<span data-ttu-id="b0e41-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b0e41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0e41-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b0e41-111">Permission type</span></span>|<span data-ttu-id="b0e41-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b0e41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0e41-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b0e41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0e41-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0e41-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b0e41-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b0e41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0e41-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0e41-116">Not supported.</span></span>|
|<span data-ttu-id="b0e41-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0e41-117">Application</span></span>|<span data-ttu-id="b0e41-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b0e41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0e41-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b0e41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## <a name="request-headers"></a><span data-ttu-id="b0e41-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e41-120">Request headers</span></span>
|<span data-ttu-id="b0e41-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b0e41-121">Header</span></span>|<span data-ttu-id="b0e41-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b0e41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0e41-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b0e41-123">Authorization</span></span>|<span data-ttu-id="b0e41-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b0e41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0e41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0e41-125">Accept</span></span>|<span data-ttu-id="b0e41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0e41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0e41-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e41-127">Request body</span></span>
<span data-ttu-id="b0e41-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b0e41-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b0e41-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0e41-129">Response</span></span>
<span data-ttu-id="b0e41-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b0e41-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b0e41-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b0e41-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0e41-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b0e41-132">Request</span></span>
<span data-ttu-id="b0e41-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b0e41-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

### <a name="response"></a><span data-ttu-id="b0e41-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b0e41-134">Response</span></span>
<span data-ttu-id="b0e41-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b0e41-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





