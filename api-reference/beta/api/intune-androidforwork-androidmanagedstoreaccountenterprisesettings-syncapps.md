---
title: Ação syncApps
description: Ainda não documentado
ms.openlocfilehash: 8c9e25c53204299e8c36d6d004ea2c2fd56066c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037250"
---
# <a name="syncapps-action"></a><span data-ttu-id="45100-103">Ação syncApps</span><span class="sxs-lookup"><span data-stu-id="45100-103">syncApps action</span></span>

> <span data-ttu-id="45100-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45100-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45100-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45100-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45100-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="45100-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45100-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="45100-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45100-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="45100-108">Prerequisites</span></span>
<span data-ttu-id="45100-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="45100-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45100-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="45100-111">Permission type</span></span>|<span data-ttu-id="45100-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="45100-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45100-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="45100-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45100-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45100-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="45100-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="45100-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45100-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45100-116">Not supported.</span></span>|
|<span data-ttu-id="45100-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="45100-117">Application</span></span>|<span data-ttu-id="45100-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="45100-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45100-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="45100-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/syncApps
```

## <a name="request-headers"></a><span data-ttu-id="45100-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="45100-120">Request headers</span></span>
|<span data-ttu-id="45100-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="45100-121">Header</span></span>|<span data-ttu-id="45100-122">Valor</span><span class="sxs-lookup"><span data-stu-id="45100-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45100-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="45100-123">Authorization</span></span>|<span data-ttu-id="45100-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="45100-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45100-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45100-125">Accept</span></span>|<span data-ttu-id="45100-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45100-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45100-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="45100-127">Request body</span></span>
<span data-ttu-id="45100-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="45100-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45100-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="45100-129">Response</span></span>
<span data-ttu-id="45100-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="45100-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="45100-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="45100-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="45100-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="45100-132">Request</span></span>
<span data-ttu-id="45100-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="45100-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/syncApps
```

### <a name="response"></a><span data-ttu-id="45100-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="45100-134">Response</span></span>
<span data-ttu-id="45100-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="45100-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





