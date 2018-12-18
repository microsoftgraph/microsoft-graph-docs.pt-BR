---
title: Atualizar iosVppApp
description: Atualiza as propriedades de um objeto iosVppApp.
author: tfitzmac
ms.openlocfilehash: 05da16de7fc9d9cf5c556fd48f29d327bd6cd6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348003"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="2a508-103">Atualizar iosVppApp</span><span class="sxs-lookup"><span data-stu-id="2a508-103">Update iosVppApp</span></span>

> <span data-ttu-id="2a508-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2a508-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a508-105">Atualiza as propriedades de um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a508-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2a508-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2a508-106">Prerequisites</span></span>
<span data-ttu-id="2a508-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a508-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a508-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a508-109">Permission type</span></span>|<span data-ttu-id="2a508-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2a508-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a508-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a508-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2a508-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a508-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2a508-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a508-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a508-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a508-114">Not supported.</span></span>|
|<span data-ttu-id="2a508-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a508-115">Application</span></span>|<span data-ttu-id="2a508-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a508-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a508-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a508-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2a508-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a508-118">Request headers</span></span>
|<span data-ttu-id="2a508-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2a508-119">Header</span></span>|<span data-ttu-id="2a508-120">Valor</span><span class="sxs-lookup"><span data-stu-id="2a508-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a508-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a508-121">Authorization</span></span>|<span data-ttu-id="2a508-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a508-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a508-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2a508-123">Accept</span></span>|<span data-ttu-id="2a508-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2a508-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a508-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a508-125">Request body</span></span>
<span data-ttu-id="2a508-126">No corpo da solicitação, forneça uma representação JSON do objeto [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a508-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="2a508-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [iosVppApp](../resources/intune-apps-iosvppapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a508-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="2a508-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a508-128">Property</span></span>|<span data-ttu-id="2a508-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a508-129">Type</span></span>|<span data-ttu-id="2a508-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a508-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a508-131">id</span><span class="sxs-lookup"><span data-stu-id="2a508-131">id</span></span>|<span data-ttu-id="2a508-132">String</span><span class="sxs-lookup"><span data-stu-id="2a508-132">String</span></span>|<span data-ttu-id="2a508-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="2a508-133">Key of the entity.</span></span> <span data-ttu-id="2a508-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2a508-135">displayName</span></span>|<span data-ttu-id="2a508-136">String</span><span class="sxs-lookup"><span data-stu-id="2a508-136">String</span></span>|<span data-ttu-id="2a508-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="2a508-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2a508-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-139">description</span><span class="sxs-lookup"><span data-stu-id="2a508-139">description</span></span>|<span data-ttu-id="2a508-140">String</span><span class="sxs-lookup"><span data-stu-id="2a508-140">String</span></span>|<span data-ttu-id="2a508-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a508-141">The description of the app.</span></span> <span data-ttu-id="2a508-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-143">publisher</span><span class="sxs-lookup"><span data-stu-id="2a508-143">publisher</span></span>|<span data-ttu-id="2a508-144">String</span><span class="sxs-lookup"><span data-stu-id="2a508-144">String</span></span>|<span data-ttu-id="2a508-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a508-145">The publisher of the app.</span></span> <span data-ttu-id="2a508-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2a508-147">largeIcon</span></span>|[<span data-ttu-id="2a508-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2a508-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2a508-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="2a508-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2a508-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2a508-151">createdDateTime</span></span>|<span data-ttu-id="2a508-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a508-152">DateTimeOffset</span></span>|<span data-ttu-id="2a508-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a508-153">The date and time the app was created.</span></span> <span data-ttu-id="2a508-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a508-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2a508-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a508-156">DateTimeOffset</span></span>|<span data-ttu-id="2a508-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="2a508-157">The date and time the app was last modified.</span></span> <span data-ttu-id="2a508-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2a508-159">isFeatured</span></span>|<span data-ttu-id="2a508-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2a508-160">Boolean</span></span>|<span data-ttu-id="2a508-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2a508-162">privacyInformationUrl</span></span>|<span data-ttu-id="2a508-163">String</span><span class="sxs-lookup"><span data-stu-id="2a508-163">String</span></span>|<span data-ttu-id="2a508-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2a508-164">The privacy statement Url.</span></span> <span data-ttu-id="2a508-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2a508-166">informationUrl</span></span>|<span data-ttu-id="2a508-167">String</span><span class="sxs-lookup"><span data-stu-id="2a508-167">String</span></span>|<span data-ttu-id="2a508-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="2a508-168">The more information Url.</span></span> <span data-ttu-id="2a508-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-170">owner</span><span class="sxs-lookup"><span data-stu-id="2a508-170">owner</span></span>|<span data-ttu-id="2a508-171">String</span><span class="sxs-lookup"><span data-stu-id="2a508-171">String</span></span>|<span data-ttu-id="2a508-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="2a508-172">The owner of the app.</span></span> <span data-ttu-id="2a508-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-174">developer</span><span class="sxs-lookup"><span data-stu-id="2a508-174">developer</span></span>|<span data-ttu-id="2a508-175">String</span><span class="sxs-lookup"><span data-stu-id="2a508-175">String</span></span>|<span data-ttu-id="2a508-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a508-176">The developer of the app.</span></span> <span data-ttu-id="2a508-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-178">Observações</span><span class="sxs-lookup"><span data-stu-id="2a508-178">notes</span></span>|<span data-ttu-id="2a508-179">String</span><span class="sxs-lookup"><span data-stu-id="2a508-179">String</span></span>|<span data-ttu-id="2a508-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a508-180">Notes for the app.</span></span> <span data-ttu-id="2a508-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="2a508-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2a508-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="2a508-182">publishingState</span></span>|[<span data-ttu-id="2a508-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2a508-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2a508-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2a508-184">The publishing state for the app.</span></span> <span data-ttu-id="2a508-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="2a508-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2a508-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="2a508-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2a508-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="2a508-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2a508-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2a508-188">usedLicenseCount</span></span>|<span data-ttu-id="2a508-189">Int32</span><span class="sxs-lookup"><span data-stu-id="2a508-189">Int32</span></span>|<span data-ttu-id="2a508-190">O número de aplicativos VPP em uso.</span><span class="sxs-lookup"><span data-stu-id="2a508-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="2a508-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="2a508-191">totalLicenseCount</span></span>|<span data-ttu-id="2a508-192">Int32</span><span class="sxs-lookup"><span data-stu-id="2a508-192">Int32</span></span>|<span data-ttu-id="2a508-193">O número total de licenças VPP.</span><span class="sxs-lookup"><span data-stu-id="2a508-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="2a508-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="2a508-194">releaseDateTime</span></span>|<span data-ttu-id="2a508-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a508-195">DateTimeOffset</span></span>|<span data-ttu-id="2a508-196">A data e a hora de lançamento do aplicativo VPP.</span><span class="sxs-lookup"><span data-stu-id="2a508-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="2a508-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="2a508-197">appStoreUrl</span></span>|<span data-ttu-id="2a508-198">String</span><span class="sxs-lookup"><span data-stu-id="2a508-198">String</span></span>|<span data-ttu-id="2a508-199">A URL da loja.</span><span class="sxs-lookup"><span data-stu-id="2a508-199">The store URL.</span></span>|
|<span data-ttu-id="2a508-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="2a508-200">licensingType</span></span>|[<span data-ttu-id="2a508-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="2a508-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="2a508-202">O tipo de licença com suporte.</span><span class="sxs-lookup"><span data-stu-id="2a508-202">The supported License Type.</span></span>|
|<span data-ttu-id="2a508-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a508-203">applicableDeviceType</span></span>|[<span data-ttu-id="2a508-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="2a508-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="2a508-205">O tipo de dispositivo iOS aplicável.</span><span class="sxs-lookup"><span data-stu-id="2a508-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="2a508-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="2a508-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="2a508-207">String</span><span class="sxs-lookup"><span data-stu-id="2a508-207">String</span></span>|<span data-ttu-id="2a508-208">A organização associada ao Token do Programa de Compra por Volume da Apple</span><span class="sxs-lookup"><span data-stu-id="2a508-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="2a508-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2a508-209">vppTokenAccountType</span></span>|[<span data-ttu-id="2a508-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="2a508-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="2a508-211">O tipo de programa de compra por volume ao qual o Token do Programa de Compra por Volume da Apple especificado está associado.</span><span class="sxs-lookup"><span data-stu-id="2a508-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="2a508-212">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2a508-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="2a508-213">Os valores possíveis são: `business`, `education`.</span><span class="sxs-lookup"><span data-stu-id="2a508-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="2a508-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="2a508-214">vppTokenAppleId</span></span>|<span data-ttu-id="2a508-215">String</span><span class="sxs-lookup"><span data-stu-id="2a508-215">String</span></span>|<span data-ttu-id="2a508-216">O Apple Id associado ao Token do Programa de Compra de Volume da Apple.</span><span class="sxs-lookup"><span data-stu-id="2a508-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="2a508-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="2a508-217">bundleId</span></span>|<span data-ttu-id="2a508-218">String</span><span class="sxs-lookup"><span data-stu-id="2a508-218">String</span></span>|<span data-ttu-id="2a508-219">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2a508-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="2a508-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a508-220">Response</span></span>
<span data-ttu-id="2a508-221">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [iosVppApp](../resources/intune-apps-iosvppapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a508-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a508-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2a508-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="2a508-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a508-223">Request</span></span>
<span data-ttu-id="2a508-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a508-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a508-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a508-225">Response</span></span>
<span data-ttu-id="2a508-p116">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a508-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



