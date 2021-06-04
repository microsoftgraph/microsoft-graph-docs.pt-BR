---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 32859d9fce2e53e3f1559717189d6dce1ec279be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754459"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="72b2f-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="72b2f-103">Update iosVppApp</span></span>

<span data-ttu-id="72b2f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b2f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72b2f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72b2f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72b2f-106">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="72b2f-106">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72b2f-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="72b2f-107">Prerequisites</span></span>
<span data-ttu-id="72b2f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="72b2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72b2f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="72b2f-110">Permission type</span></span>|<span data-ttu-id="72b2f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="72b2f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72b2f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="72b2f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72b2f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72b2f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="72b2f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="72b2f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72b2f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="72b2f-115">Not supported.</span></span>|
|<span data-ttu-id="72b2f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="72b2f-116">Application</span></span>|<span data-ttu-id="72b2f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72b2f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="72b2f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="72b2f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="72b2f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="72b2f-119">Request headers</span></span>
|<span data-ttu-id="72b2f-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="72b2f-120">Header</span></span>|<span data-ttu-id="72b2f-121">Valor</span><span class="sxs-lookup"><span data-stu-id="72b2f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72b2f-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="72b2f-122">Authorization</span></span>|<span data-ttu-id="72b2f-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72b2f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72b2f-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="72b2f-124">Accept</span></span>|<span data-ttu-id="72b2f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72b2f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72b2f-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="72b2f-126">Request body</span></span>
<span data-ttu-id="72b2f-127">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="72b2f-127">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="72b2f-128">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="72b2f-128">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="72b2f-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72b2f-129">Property</span></span>|<span data-ttu-id="72b2f-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="72b2f-130">Type</span></span>|<span data-ttu-id="72b2f-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="72b2f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b2f-132">id</span><span class="sxs-lookup"><span data-stu-id="72b2f-132">id</span></span>|<span data-ttu-id="72b2f-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b2f-133">String</span></span>|<span data-ttu-id="72b2f-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="72b2f-134">Key of the entity.</span></span> <span data-ttu-id="72b2f-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="72b2f-136">displayName</span></span>|<span data-ttu-id="72b2f-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b2f-137">String</span></span>|<span data-ttu-id="72b2f-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="72b2f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="72b2f-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-140">descrição</span><span class="sxs-lookup"><span data-stu-id="72b2f-140">description</span></span>|<span data-ttu-id="72b2f-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b2f-141">String</span></span>|<span data-ttu-id="72b2f-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-142">The description of the app.</span></span> <span data-ttu-id="72b2f-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-144">publicador</span><span class="sxs-lookup"><span data-stu-id="72b2f-144">publisher</span></span>|<span data-ttu-id="72b2f-145">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-145">String</span></span>|<span data-ttu-id="72b2f-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-146">The publisher of the app.</span></span> <span data-ttu-id="72b2f-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="72b2f-148">largeIcon</span></span>|[<span data-ttu-id="72b2f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="72b2f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="72b2f-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="72b2f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="72b2f-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72b2f-152">createdDateTime</span></span>|<span data-ttu-id="72b2f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b2f-153">DateTimeOffset</span></span>|<span data-ttu-id="72b2f-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-154">The date and time the app was created.</span></span> <span data-ttu-id="72b2f-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72b2f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="72b2f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b2f-157">DateTimeOffset</span></span>|<span data-ttu-id="72b2f-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="72b2f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="72b2f-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="72b2f-160">isFeatured</span></span>|<span data-ttu-id="72b2f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="72b2f-161">Boolean</span></span>|<span data-ttu-id="72b2f-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="72b2f-163">privacyInformationUrl</span></span>|<span data-ttu-id="72b2f-164">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-164">String</span></span>|<span data-ttu-id="72b2f-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="72b2f-165">The privacy statement Url.</span></span> <span data-ttu-id="72b2f-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="72b2f-167">informationUrl</span></span>|<span data-ttu-id="72b2f-168">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-168">String</span></span>|<span data-ttu-id="72b2f-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="72b2f-169">The more information Url.</span></span> <span data-ttu-id="72b2f-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="72b2f-171">owner</span></span>|<span data-ttu-id="72b2f-172">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="72b2f-172">String</span></span>|<span data-ttu-id="72b2f-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-173">The owner of the app.</span></span> <span data-ttu-id="72b2f-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-175">developer</span><span class="sxs-lookup"><span data-stu-id="72b2f-175">developer</span></span>|<span data-ttu-id="72b2f-176">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-176">String</span></span>|<span data-ttu-id="72b2f-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-177">The developer of the app.</span></span> <span data-ttu-id="72b2f-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-179">notes</span><span class="sxs-lookup"><span data-stu-id="72b2f-179">notes</span></span>|<span data-ttu-id="72b2f-180">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-180">String</span></span>|<span data-ttu-id="72b2f-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-181">Notes for the app.</span></span> <span data-ttu-id="72b2f-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="72b2f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="72b2f-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="72b2f-183">publishingState</span></span>|[<span data-ttu-id="72b2f-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="72b2f-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="72b2f-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="72b2f-185">The publishing state for the app.</span></span> <span data-ttu-id="72b2f-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="72b2f-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="72b2f-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="72b2f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="72b2f-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="72b2f-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="72b2f-189">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="72b2f-189">usedLicenseCount</span></span>|<span data-ttu-id="72b2f-190">Int32</span><span class="sxs-lookup"><span data-stu-id="72b2f-190">Int32</span></span>|<span data-ttu-id="72b2f-191">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="72b2f-191">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="72b2f-192">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="72b2f-192">totalLicenseCount</span></span>|<span data-ttu-id="72b2f-193">Int32</span><span class="sxs-lookup"><span data-stu-id="72b2f-193">Int32</span></span>|<span data-ttu-id="72b2f-194">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="72b2f-194">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="72b2f-195">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="72b2f-195">releaseDateTime</span></span>|<span data-ttu-id="72b2f-196">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b2f-196">DateTimeOffset</span></span>|<span data-ttu-id="72b2f-197">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="72b2f-197">The VPP application release date and time.</span></span>|
|<span data-ttu-id="72b2f-198">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="72b2f-198">appStoreUrl</span></span>|<span data-ttu-id="72b2f-199">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-199">String</span></span>|<span data-ttu-id="72b2f-200">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="72b2f-200">The store URL.</span></span>|
|<span data-ttu-id="72b2f-201">licensingType</span><span class="sxs-lookup"><span data-stu-id="72b2f-201">licensingType</span></span>|[<span data-ttu-id="72b2f-202">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="72b2f-202">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="72b2f-203">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="72b2f-203">The supported License Type.</span></span>|
|<span data-ttu-id="72b2f-204">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="72b2f-204">applicableDeviceType</span></span>|[<span data-ttu-id="72b2f-205">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="72b2f-205">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="72b2f-206">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="72b2f-206">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="72b2f-207">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="72b2f-207">vppTokenOrganizationName</span></span>|<span data-ttu-id="72b2f-208">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-208">String</span></span>|<span data-ttu-id="72b2f-209">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="72b2f-209">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="72b2f-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="72b2f-210">vppTokenAccountType</span></span>|[<span data-ttu-id="72b2f-211">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="72b2f-211">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="72b2f-212">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="72b2f-212">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="72b2f-213">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="72b2f-213">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="72b2f-214">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="72b2f-214">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="72b2f-215">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="72b2f-215">vppTokenAppleId</span></span>|<span data-ttu-id="72b2f-216">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-216">String</span></span>|<span data-ttu-id="72b2f-217">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="72b2f-217">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="72b2f-218">bundleId</span><span class="sxs-lookup"><span data-stu-id="72b2f-218">bundleId</span></span>|<span data-ttu-id="72b2f-219">String</span><span class="sxs-lookup"><span data-stu-id="72b2f-219">String</span></span>|<span data-ttu-id="72b2f-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="72b2f-220">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="72b2f-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="72b2f-221">Response</span></span>
<span data-ttu-id="72b2f-222">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="72b2f-222">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72b2f-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="72b2f-223">Example</span></span>

### <a name="request"></a><span data-ttu-id="72b2f-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="72b2f-224">Request</span></span>
<span data-ttu-id="72b2f-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="72b2f-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1222

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="72b2f-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="72b2f-226">Response</span></span>
<span data-ttu-id="72b2f-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="72b2f-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1394

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value"
}
```




