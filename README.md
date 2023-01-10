
index.tsx

type UserWalletType = {
title: string
amount: number
}
type UserWalletPropsType = {
wallet: UserWalletType
}
export const UserMoney: React.FC<UserWalletPropsType> = (props: UserWalletPropsType) => {

    const wallets = [
        {title: 'bitcoin', amount: 1},
        {title: '$', amount: 100}
    ]

    return <div>
        <UserWallet wallet={wallets[0]} />
        <UserWallet wallet={wallets[1]} />
    </div>
}

export const UserWallet: React.FC<UserWalletPropsType> = (props) => {
return <div>title: {props.wallet.title}, amount: {props.wallet.amount}</div>
}

___________________________________________ Monday Week 2 