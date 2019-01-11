---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 66d94d9bca1d83ba8d99afb218451667848f90e7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813234"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="9968c-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="9968c-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="9968c-104">**Observação:** o uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9968c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9968c-105">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9968c-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9968c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9968c-106">Prerequisites</span></span>
<span data-ttu-id="9968c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9968c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9968c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9968c-109">Permission type</span></span>|<span data-ttu-id="9968c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9968c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9968c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9968c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9968c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9968c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9968c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9968c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9968c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9968c-114">Not supported.</span></span>|
|<span data-ttu-id="9968c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9968c-115">Application</span></span>|<span data-ttu-id="9968c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9968c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9968c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9968c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="9968c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9968c-118">Request headers</span></span>
|<span data-ttu-id="9968c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9968c-119">Header</span></span>|<span data-ttu-id="9968c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="9968c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9968c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="9968c-121">Authorization</span></span>|<span data-ttu-id="9968c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9968c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9968c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9968c-123">Accept</span></span>|<span data-ttu-id="9968c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9968c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9968c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9968c-125">Request body</span></span>
<span data-ttu-id="9968c-126">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9968c-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="9968c-127">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="9968c-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="9968c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9968c-128">Property</span></span>|<span data-ttu-id="9968c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="9968c-129">Type</span></span>|<span data-ttu-id="9968c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="9968c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9968c-131">id</span><span class="sxs-lookup"><span data-stu-id="9968c-131">id</span></span>|<span data-ttu-id="9968c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-132">String</span></span>|<span data-ttu-id="9968c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9968c-133">Key of the entity.</span></span> <span data-ttu-id="9968c-134">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="9968c-135">displayName</span></span>|<span data-ttu-id="9968c-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-136">String</span></span>|<span data-ttu-id="9968c-137">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="9968c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="9968c-138">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-139">description</span><span class="sxs-lookup"><span data-stu-id="9968c-139">description</span></span>|<span data-ttu-id="9968c-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-140">String</span></span>|<span data-ttu-id="9968c-141">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-141">The description of the app.</span></span> <span data-ttu-id="9968c-142">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-143">publisher</span><span class="sxs-lookup"><span data-stu-id="9968c-143">publisher</span></span>|<span data-ttu-id="9968c-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-144">String</span></span>|<span data-ttu-id="9968c-145">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-145">The publisher of the app.</span></span> <span data-ttu-id="9968c-146">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="9968c-147">largeIcon</span></span>|[<span data-ttu-id="9968c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="9968c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="9968c-149">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="9968c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="9968c-150">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9968c-151">createdDateTime</span></span>|<span data-ttu-id="9968c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9968c-152">DateTimeOffset</span></span>|<span data-ttu-id="9968c-153">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-153">The date and time the app was created.</span></span> <span data-ttu-id="9968c-154">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9968c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="9968c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9968c-156">DateTimeOffset</span></span>|<span data-ttu-id="9968c-157">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="9968c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="9968c-158">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="9968c-159">isFeatured</span></span>|<span data-ttu-id="9968c-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="9968c-160">Boolean</span></span>|<span data-ttu-id="9968c-161">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="9968c-162">privacyInformationUrl</span></span>|<span data-ttu-id="9968c-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-163">String</span></span>|<span data-ttu-id="9968c-164">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9968c-164">The privacy statement Url.</span></span> <span data-ttu-id="9968c-165">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="9968c-166">informationUrl</span></span>|<span data-ttu-id="9968c-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-167">String</span></span>|<span data-ttu-id="9968c-168">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="9968c-168">The more information Url.</span></span> <span data-ttu-id="9968c-169">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-170">owner</span><span class="sxs-lookup"><span data-stu-id="9968c-170">owner</span></span>|<span data-ttu-id="9968c-171">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-171">String</span></span>|<span data-ttu-id="9968c-172">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="9968c-172">The owner of the app.</span></span> <span data-ttu-id="9968c-173">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-174">developer</span><span class="sxs-lookup"><span data-stu-id="9968c-174">developer</span></span>|<span data-ttu-id="9968c-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-175">String</span></span>|<span data-ttu-id="9968c-176">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-176">The developer of the app.</span></span> <span data-ttu-id="9968c-177">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-178">Observações</span><span class="sxs-lookup"><span data-stu-id="9968c-178">notes</span></span>|<span data-ttu-id="9968c-179">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-179">String</span></span>|<span data-ttu-id="9968c-180">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-180">Notes for the app.</span></span> <span data-ttu-id="9968c-181">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="9968c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="9968c-182">publishingState</span></span>|[<span data-ttu-id="9968c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="9968c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="9968c-184">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-184">The publishing state for the app.</span></span> <span data-ttu-id="9968c-185">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="9968c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="9968c-186">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="9968c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="9968c-187">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="9968c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="9968c-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="9968c-188">appAvailability</span></span>|[<span data-ttu-id="9968c-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="9968c-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="9968c-190">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-190">The Application's availability.</span></span> <span data-ttu-id="9968c-191">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="9968c-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="9968c-192">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="9968c-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="9968c-193">version</span><span class="sxs-lookup"><span data-stu-id="9968c-193">version</span></span>|<span data-ttu-id="9968c-194">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-194">String</span></span>|<span data-ttu-id="9968c-195">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9968c-195">The Application's version.</span></span> <span data-ttu-id="9968c-196">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="9968c-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="9968c-197">committedContentVersion</span></span>|<span data-ttu-id="9968c-198">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-198">String</span></span>|<span data-ttu-id="9968c-199">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="9968c-199">The internal committed content version.</span></span> <span data-ttu-id="9968c-200">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="9968c-201">fileName</span><span class="sxs-lookup"><span data-stu-id="9968c-201">fileName</span></span>|<span data-ttu-id="9968c-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-202">String</span></span>|<span data-ttu-id="9968c-203">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="9968c-203">The name of the main Lob application file.</span></span> <span data-ttu-id="9968c-204">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="9968c-205">size</span><span class="sxs-lookup"><span data-stu-id="9968c-205">size</span></span>|<span data-ttu-id="9968c-206">Int64</span><span class="sxs-lookup"><span data-stu-id="9968c-206">Int64</span></span>|<span data-ttu-id="9968c-207">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="9968c-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="9968c-208">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="9968c-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="9968c-209">packageId</span><span class="sxs-lookup"><span data-stu-id="9968c-209">packageId</span></span>|<span data-ttu-id="9968c-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-210">String</span></span>|<span data-ttu-id="9968c-211">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="9968c-211">The package identifier.</span></span>|
|<span data-ttu-id="9968c-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9968c-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9968c-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9968c-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="9968c-214">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="9968c-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="9968c-215">versionName</span><span class="sxs-lookup"><span data-stu-id="9968c-215">versionName</span></span>|<span data-ttu-id="9968c-216">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-216">String</span></span>|<span data-ttu-id="9968c-217">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="9968c-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="9968c-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="9968c-218">versionCode</span></span>|<span data-ttu-id="9968c-219">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9968c-219">String</span></span>|<span data-ttu-id="9968c-220">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="9968c-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="9968c-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="9968c-221">Response</span></span>
<span data-ttu-id="9968c-222">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9968c-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9968c-223">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9968c-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="9968c-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9968c-224">Request</span></span>
<span data-ttu-id="9968c-225">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9968c-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="9968c-226">Resposta</span><span class="sxs-lookup"><span data-stu-id="9968c-226">Response</span></span>
<span data-ttu-id="9968c-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9968c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



