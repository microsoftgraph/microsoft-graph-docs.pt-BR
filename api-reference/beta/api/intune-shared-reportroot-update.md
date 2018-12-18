---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: tfitzmac
ms.openlocfilehash: 4f3d0e297a9b7d122e9b21afd7555c1af307d2d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349529"
---
# <a name="update-reportroot"></a><span data-ttu-id="77091-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="77091-103">Update reportRoot</span></span>

> <span data-ttu-id="77091-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="77091-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="77091-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="77091-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77091-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="77091-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="77091-107">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="77091-107">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="77091-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="77091-108">Prerequisites</span></span>
<span data-ttu-id="77091-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77091-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="77091-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77091-111">Permission type</span></span>|<span data-ttu-id="77091-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="77091-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77091-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77091-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="77091-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="77091-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="77091-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77091-115">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="77091-116">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="77091-116">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="77091-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77091-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="77091-118">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77091-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77091-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77091-119">Not supported.</span></span>|
|<span data-ttu-id="77091-120">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77091-120">Application</span></span>|<span data-ttu-id="77091-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="77091-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77091-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77091-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="77091-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77091-123">Request headers</span></span>
|<span data-ttu-id="77091-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="77091-124">Header</span></span>|<span data-ttu-id="77091-125">Valor</span><span class="sxs-lookup"><span data-stu-id="77091-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77091-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="77091-126">Authorization</span></span>|<span data-ttu-id="77091-127">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77091-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77091-128">Accept</span><span class="sxs-lookup"><span data-stu-id="77091-128">Accept</span></span>|<span data-ttu-id="77091-129">application/json</span><span class="sxs-lookup"><span data-stu-id="77091-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77091-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77091-130">Request body</span></span>
<span data-ttu-id="77091-131">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="77091-131">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="77091-132">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="77091-132">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="77091-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77091-133">Property</span></span>|<span data-ttu-id="77091-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="77091-134">Type</span></span>|<span data-ttu-id="77091-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="77091-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77091-136">id</span><span class="sxs-lookup"><span data-stu-id="77091-136">id</span></span>|<span data-ttu-id="77091-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77091-137">String</span></span>|<span data-ttu-id="77091-138">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="77091-138">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="77091-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77091-139">Response</span></span>
<span data-ttu-id="77091-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77091-140">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77091-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77091-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="77091-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77091-142">Request</span></span>
<span data-ttu-id="77091-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77091-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="77091-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="77091-144">Response</span></span>
<span data-ttu-id="77091-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77091-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```



