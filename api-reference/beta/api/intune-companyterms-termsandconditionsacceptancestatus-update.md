---
title: Atualizar termsAndConditionsAcceptanceStatus
description: Atualizar as propriedades de um objeto termsAndConditionsAcceptanceStatus.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 886910cfe2ac0b1bcf6ad1fcbd0a76a79c515aba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858433"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="db16e-103">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="db16e-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="db16e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="db16e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db16e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="db16e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db16e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="db16e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db16e-107">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="db16e-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db16e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="db16e-108">Prerequisites</span></span>
<span data-ttu-id="db16e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="db16e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db16e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="db16e-111">Permission type</span></span>|<span data-ttu-id="db16e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="db16e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db16e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="db16e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="db16e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db16e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="db16e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="db16e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db16e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db16e-116">Not supported.</span></span>|
|<span data-ttu-id="db16e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="db16e-117">Application</span></span>|<span data-ttu-id="db16e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="db16e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db16e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="db16e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="db16e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="db16e-120">Request headers</span></span>
|<span data-ttu-id="db16e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="db16e-121">Header</span></span>|<span data-ttu-id="db16e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="db16e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db16e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="db16e-123">Authorization</span></span>|<span data-ttu-id="db16e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="db16e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db16e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="db16e-125">Accept</span></span>|<span data-ttu-id="db16e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="db16e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db16e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="db16e-127">Request body</span></span>
<span data-ttu-id="db16e-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="db16e-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="db16e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="db16e-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="db16e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db16e-130">Property</span></span>|<span data-ttu-id="db16e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="db16e-131">Type</span></span>|<span data-ttu-id="db16e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="db16e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db16e-133">id</span><span class="sxs-lookup"><span data-stu-id="db16e-133">id</span></span>|<span data-ttu-id="db16e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db16e-134">String</span></span>|<span data-ttu-id="db16e-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="db16e-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="db16e-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="db16e-136">userDisplayName</span></span>|<span data-ttu-id="db16e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="db16e-137">String</span></span>|<span data-ttu-id="db16e-138">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="db16e-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="db16e-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="db16e-139">acceptedVersion</span></span>|<span data-ttu-id="db16e-140">Int32</span><span class="sxs-lookup"><span data-stu-id="db16e-140">Int32</span></span>|<span data-ttu-id="db16e-141">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="db16e-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="db16e-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="db16e-142">acceptedDateTime</span></span>|<span data-ttu-id="db16e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db16e-143">DateTimeOffset</span></span>|<span data-ttu-id="db16e-144">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="db16e-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="db16e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="db16e-145">Response</span></span>
<span data-ttu-id="db16e-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="db16e-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db16e-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="db16e-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="db16e-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="db16e-148">Request</span></span>
<span data-ttu-id="db16e-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="db16e-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 138

{
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="db16e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="db16e-150">Response</span></span>
<span data-ttu-id="db16e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="db16e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```





