---
title: Atualizar reportRoot
description: Atualizar as propriedades de um objeto reportRoot.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ca91c074e19887d889ac8bed332055f36ebed08d
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48694176"
---
# <a name="update-reportroot"></a><span data-ttu-id="b00ce-103">Atualizar reportRoot</span><span class="sxs-lookup"><span data-stu-id="b00ce-103">Update reportRoot</span></span>

<span data-ttu-id="b00ce-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b00ce-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b00ce-105">**Importante:** As APIs na versão/beta no Microsoft Graph estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b00ce-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b00ce-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b00ce-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b00ce-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b00ce-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b00ce-108">Atualizar as propriedades de um objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b00ce-108">Update the properties of a [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b00ce-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b00ce-109">Prerequisites</span></span>
<span data-ttu-id="b00ce-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b00ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b00ce-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b00ce-112">Permission type</span></span>|<span data-ttu-id="b00ce-113">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b00ce-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b00ce-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b00ce-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="b00ce-115">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b00ce-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b00ce-116">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b00ce-116">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b00ce-117">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b00ce-117">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b00ce-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b00ce-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b00ce-119">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b00ce-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b00ce-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b00ce-120">Not supported.</span></span>|
|<span data-ttu-id="b00ce-121">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b00ce-121">Application</span></span>||
| <span data-ttu-id="b00ce-122">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="b00ce-122">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="b00ce-123">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b00ce-123">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="b00ce-124">&nbsp; &nbsp; **Solução de problemas**</span><span class="sxs-lookup"><span data-stu-id="b00ce-124">&nbsp; &nbsp; **Troubleshooting**</span></span> | <span data-ttu-id="b00ce-125">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b00ce-125">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b00ce-126">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b00ce-126">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="b00ce-127">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b00ce-127">Request headers</span></span>
|<span data-ttu-id="b00ce-128">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b00ce-128">Header</span></span>|<span data-ttu-id="b00ce-129">Valor</span><span class="sxs-lookup"><span data-stu-id="b00ce-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b00ce-130">Autorização</span><span class="sxs-lookup"><span data-stu-id="b00ce-130">Authorization</span></span>|<span data-ttu-id="b00ce-131">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b00ce-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b00ce-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b00ce-132">Accept</span></span>|<span data-ttu-id="b00ce-133">application/json</span><span class="sxs-lookup"><span data-stu-id="b00ce-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b00ce-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b00ce-134">Request body</span></span>
<span data-ttu-id="b00ce-135">No corpo da solicitação, forneça uma representação JSON do objeto [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b00ce-135">In the request body, supply a JSON representation for the [reportRoot](../resources/intune-shared-reportroot.md) object.</span></span>

<span data-ttu-id="b00ce-136">A tabela a seguir mostra as propriedades que são necessárias ao criar [reportRoot](../resources/intune-shared-reportroot.md).</span><span class="sxs-lookup"><span data-stu-id="b00ce-136">The following table shows the properties that are required when you create the [reportRoot](../resources/intune-shared-reportroot.md).</span></span>

|<span data-ttu-id="b00ce-137">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b00ce-137">Property</span></span>|<span data-ttu-id="b00ce-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="b00ce-138">Type</span></span>|<span data-ttu-id="b00ce-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b00ce-139">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b00ce-140">id</span><span class="sxs-lookup"><span data-stu-id="b00ce-140">id</span></span>|<span data-ttu-id="b00ce-141">String</span><span class="sxs-lookup"><span data-stu-id="b00ce-141">String</span></span>|<span data-ttu-id="b00ce-142">O identificador exclusivo dessa entidade.</span><span class="sxs-lookup"><span data-stu-id="b00ce-142">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="b00ce-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="b00ce-143">Response</span></span>
<span data-ttu-id="b00ce-144">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [reportRoot](../resources/intune-shared-reportroot.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b00ce-144">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune-shared-reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b00ce-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b00ce-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b00ce-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b00ce-146">Request</span></span>
<span data-ttu-id="b00ce-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b00ce-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="b00ce-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="b00ce-148">Response</span></span>
<span data-ttu-id="b00ce-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b00ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```











