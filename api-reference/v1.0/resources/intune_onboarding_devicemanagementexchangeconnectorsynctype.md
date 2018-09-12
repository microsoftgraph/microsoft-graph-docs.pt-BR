# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a><span data-ttu-id="b65f5-101">tipo enumerado deviceManagementExchangeConnectorSyncType</span><span class="sxs-lookup"><span data-stu-id="b65f5-101">deviceManagementExchangeConnectorSyncType enum type</span></span>

> <span data-ttu-id="b65f5-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b65f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b65f5-103">O tipo de sincronização solicitada do Exchange Connector.</span><span class="sxs-lookup"><span data-stu-id="b65f5-103">The type of Exchange Connector Configured.</span></span>
## <a name="members"></a><span data-ttu-id="b65f5-104">Membros</span><span class="sxs-lookup"><span data-stu-id="b65f5-104">Members</span></span>
|<span data-ttu-id="b65f5-105">Membro</span><span class="sxs-lookup"><span data-stu-id="b65f5-105">Member</span></span>|<span data-ttu-id="b65f5-106">Valor</span><span class="sxs-lookup"><span data-stu-id="b65f5-106">Value</span></span>|<span data-ttu-id="b65f5-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b65f5-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b65f5-108">fullSync</span><span class="sxs-lookup"><span data-stu-id="b65f5-108">fullSync</span></span>|<span data-ttu-id="b65f5-109">0</span><span class="sxs-lookup"><span data-stu-id="b65f5-109">0%</span></span>|<span data-ttu-id="b65f5-110">Descobrir todo o dispositivo no Exchange.</span><span class="sxs-lookup"><span data-stu-id="b65f5-110">Discover all the device in Exchange.</span></span>|
|<span data-ttu-id="b65f5-111">deltaSync</span><span class="sxs-lookup"><span data-stu-id="b65f5-111">deltaSync</span></span>|<span data-ttu-id="b65f5-112">1</span><span class="sxs-lookup"><span data-stu-id="b65f5-112">-1</span></span>|<span data-ttu-id="b65f5-113">Descobrir no Exchange somente o dispositivo que foi atualizado durante a janela de sincronização delta.</span><span class="sxs-lookup"><span data-stu-id="b65f5-113">Discover only the device in Exchange which have updated during the delta sync window.</span></span>|








