# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="038e7-101">tipo enumerado sharedPCAccountDeletionPolicyType</span><span class="sxs-lookup"><span data-stu-id="038e7-101">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="038e7-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="038e7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="038e7-103">Valores possíveis para quando contas são excluídas em um PC compartilhado.</span><span class="sxs-lookup"><span data-stu-id="038e7-103">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="038e7-104">Membros</span><span class="sxs-lookup"><span data-stu-id="038e7-104">Members</span></span>
|<span data-ttu-id="038e7-105">Membro</span><span class="sxs-lookup"><span data-stu-id="038e7-105">Member</span></span>|<span data-ttu-id="038e7-106">Valor</span><span class="sxs-lookup"><span data-stu-id="038e7-106">Value</span></span>|<span data-ttu-id="038e7-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="038e7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="038e7-108">imediato</span><span class="sxs-lookup"><span data-stu-id="038e7-108">   [-immediate]</span></span>|<span data-ttu-id="038e7-109">0</span><span class="sxs-lookup"><span data-stu-id="038e7-109">0%</span></span>|<span data-ttu-id="038e7-110">Excluir imediatamente.</span><span class="sxs-lookup"><span data-stu-id="038e7-110">Delete immediately.</span></span>|
|<span data-ttu-id="038e7-111">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="038e7-111">diskSpaceThreshold</span></span>|<span data-ttu-id="038e7-112">1</span><span class="sxs-lookup"><span data-stu-id="038e7-112">-1</span></span>|<span data-ttu-id="038e7-113">Excluir no limite de espaço em disco.</span><span class="sxs-lookup"><span data-stu-id="038e7-113">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="038e7-114">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="038e7-114">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="038e7-115">2</span><span class="sxs-lookup"><span data-stu-id="038e7-115">-2</span></span>|<span data-ttu-id="038e7-116">Excluir no limite de espaço em disco ou no limite inativo.</span><span class="sxs-lookup"><span data-stu-id="038e7-116">Delete at disk space threshold or inactive threshold.</span></span>|








